### DOP Install on GCP

#### Description

- In this test case we will install DOP on the k8s cluster using storage class as standard.

#### Prerequisites

- Bring up 4 VM's - 1 master and 3 worker.
- Use any tool such as kops to spin up the k8s cluster. It is suggested to have k8s version >= 1.12.0.
- All the nodes of the cluster should be in healthy state.
- helm 3 should be installed on the k8s cluster.

#### Expected Output

- All the DOP pods should come in running state.
- All the pods in maya-system namespace should be running state.
- DOP UI should be accessible in any browser.

#### Testplan

- https://e2e.mayadata.io/docs/director/installation/tc-install-gpd-std

#### Test Result

| Job ID |   Test Description         | Execution Time |Test Result   |
 |---------|---------------------------| --------------|--------|
 |    <a href= "https://gitlab.mayadata.io/oep/oep-e2e-gcp/-/jobs/74564">74564</a>   |  Install DOP using helm with GPD underneath           |  Mon Apr  6 16:43:16 UTC 2020     |Pass  |
