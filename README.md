# RECONFLOW

> **Status: work in progress / placeholder.** This repository currently holds only this README - the pipeline code has not been published yet.

A planned unified reconnaissance pipeline that wraps the [ProjectDiscovery](https://github.com/projectdiscovery) toolchain (subfinder, dnsx, naabu, httpx, nuclei, and friends) behind a single command, so an entire recon workflow - asset discovery, resolution, port scanning, HTTP probing, and templated vulnerability scanning - runs end to end from one invocation.

## Intended workflow
1. **Discover** subdomains and assets (subfinder / OSINT sources)
2. **Resolve** and filter live hosts (dnsx)
3. **Scan** for open ports and services (naabu)
4. **Probe** HTTP endpoints (httpx)
5. **Assess** with templated checks (nuclei)

## Roadmap
- [ ] Publish the pipeline runner
- [ ] Config-driven tool selection and rate limiting
- [ ] Consolidated, deduplicated reporting

Until the code lands, see [SubHunter](https://github.com/keyuraghao/SubHunter) for a working, installable recon + vulnerability-scanning CLI.
