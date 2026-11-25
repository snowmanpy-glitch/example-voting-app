# Example Voting App — DevOps practice

Fork of [dockersamples/example-voting-app](https://github.com/dockersamples/example-voting-app),
used as a training ground for learning DevOps.

The application code is kept as-is. All upstream infrastructure (Dockerfiles, compose files,
Swarm stack, Kubernetes manifests, CI workflows, healthcheck scripts) was removed on purpose:
everything is being rebuilt from scratch, stage by stage.

## Services

| Service | Language | Path      |
|---------|----------|-----------|
| vote    | Python   | `vote/`   |
| result  | Node.js  | `result/` |
| worker  | .NET     | `worker/` |
| redis   | —        | —         |
| db      | Postgres | —         |

`seed-data/` contains a helper that generates test votes.

## Roadmap

- [ ] Stage 1 — Docker: own Dockerfiles, docker-compose, networks, healthchecks
- [ ] Stage 2 — CI with GitHub Actions
- [ ] Stage 3 — Azure and CD
- [ ] Stage 4 — Terraform and Ansible
- [ ] Stage 5 — Kubernetes and Helm
- [ ] Stage 6 — Monitoring

## License

Apache 2.0, see [LICENSE](LICENSE).
