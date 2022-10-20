# nats-cluster
- server起動
  - docker-compose -f nats1-cluster.yaml up
  - docker-compose -f nats2-cluster.yaml up
- client起動
  - docker run --network nats --rm -it natsio/nats-box
  - stream作成
    - nats str add -s [URL]
      - URLはnats://nats:nats1-1:4222とかnats://nats:nats2-3:4222
  - consumer作成
    - nats con add -s [URL]
 
