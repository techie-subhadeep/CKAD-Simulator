# CKAD Exam Simulator

**Host Steps:**
1. Install Kind Cluster (https://kind.sigs.k8s.io/docs/user/quick-start/#installation)
2. Run `kind export kubeconfig`
3. in the KubeConfig file replace server url `https://127.0.0.1:59147` wtih `https://kind-control-plane:6443` (Simulator is attached to the kind network it will be able to access the API host `kind-control-plane` port `6443`)

**Simulator Steps:**
1. Run the simulator using `docker-compose up`
2. Open http://localhost:6901/ in your browser
3. Username and password is `headless`
4. Run the `sudo sh ~/scripts/prep-env.sh` command to install configure environment similer to CAKD exam

## [CAKD Guidelines](./scripts/ckad-guidelines.md)
