# nats-cluster
- server起動
  - docker-compose -f nats1-cluster.yaml up
- client起動
  - docker run --network nats --rm -it natsio/nats-box
