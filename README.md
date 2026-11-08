# Awesome API Gateway & Routing Management

A curated list of awesome API Gateway, API Management, Reverse Proxy, and Routing Management solutions.

## Sector Overview & Market Dynamics

The global API Management and Gateway market is estimated at approximately **$5.6B to $7.7B** (scaling toward **$9.6B+** at a 15–25% CAGR), driven by microservices architectures, cloud-native deployments, and AI workloads. The sector exhibits **medium-to-high market fragmentation** rather than a winner-take-all monopoly: while hyperscale cloud platforms (Microsoft Azure, Google Cloud, AWS) dominate bundled public-cloud infrastructure, specialized open-core innovators (Kong, Tyk, Traefik) and open-source runtimes retain substantial developer-first and hybrid multi-cloud market share.

---

## SaaS & Managed API Gateway Solutions

| Product | Provider | Company Valuation / Revenue | Starting Pricing Tier | Free Tier Limits / Free Trial |
| :--- | :--- | :--- | :--- | :--- |
| **Azure API Management** | Microsoft | ~$3.94T Market Cap (FY24 Rev: $245B) | **$3.50 per 1M calls** (Consumption tier overage after free allotment) / **$48.04/month** (Developer Tier for non-production) | **1,000,000 API calls free per month** (forever on Consumption tier; capped at 3,000 operations and 100 products) |
| **Apigee API Management** | Google Cloud (Alphabet) | ~$3.33T Market Cap (FY24 Rev: $350B) | **$0.50/hour per region** (~$365/month Base Environment) + **$20 per 1M standard calls** (Pay-as-you-go) | **60-day free evaluation** (Evaluation organization sandbox with full enterprise proxy features; auto-expires after 60 days) |
| **Amazon API Gateway** | Amazon Web Services (Amazon) | ~$2.81T Market Cap (FY24 Rev: $638B) | **$1.00 per 1M requests** (HTTP APIs up to 300M requests/mo) / **$3.50 per 1M requests** (REST APIs) | **1,000,000 API calls free per month for 12 months** (AWS Free Tier: 1M HTTP/REST calls + 1M WebSocket messages & 750k connection mins/mo) |
| **MuleSoft Anypoint Platform** | Salesforce | ~$180B Market Cap (FY25 Rev: $41.5B) | **~$2,000/month** ($24,000/year annual contract for Anypoint Integration Starter tier) | **30-day free trial** (Hosted sandbox environment for API Designer & Code Builder; strictly non-production and resource-capped) |
| **NGINX Plus / F5 Distributed Cloud** | F5, Inc. | ~$20B Market Cap (FY24 Rev: $3.4B) | **$6,468.99/instance/year** (CDW / NGINX Plus subscription license + standard support) | **30-day free trial** (Full NGINX Plus software package with dynamic reconfiguration and active health checks; non-production) |
| **Kong Konnect** | Kong Inc. | $2.0B Valuation ($175M Series E) | **$25/month** (Konnect Plus Serverless Control Plane base tier; includes 1M requests/mo, additional calls metered) | **30-day free trial** (Full enterprise Konnect Plus features, unlimited trial gateways, and 30-day analytics retention) |
| **Tyk Cloud** | Tyk Technologies | ~$140M Valuation ($41M+ raised) | **~$600/month** (Tyk Cloud Starter tier for managed control plane & multi-data planes) | **48-hour free trial** (Full platform access including dashboard, developer portal, and governance tools with no traffic limits) |
| **Traefik Hub** | Traefik Labs | ~$50M Valuation ($11M+ raised) | Commercial quote-based starting at **~$99/month** (Team/Pro tiers for API Gateway & management) | **14-day free trial** (Full Traefik Hub feature access with no request/cluster caps; no credit card required) |

---

## Open-Source API Gateways & Runtimes

| Project | License | Primary Language / Architecture | Key Highlights |
| :--- | :--- | :--- | :--- |
| **[Apache APISIX](https://apisix.apache.org/)** | Apache-2.0 | NGINX + LuaJIT / etcd | Ultra-high performance, dynamic routing via etcd, multi-language plugins (Lua, Java, Go, Python, Wasm), built-in dashboard. |
| **[Kong Gateway (OSS)](https://github.com/Kong/kong)** | Apache-2.0 | OpenResty (NGINX + LuaJIT) | World's most popular open-source API gateway; extensive plugin ecosystem, DB-less & hybrid modes, Kubernetes Ingress Controller. |
| **[Envoy Gateway](https://gateway.envoyproxy.io/)** | Apache-2.0 | C++ (Envoy core) / Go (Control plane) | CNCF Kubernetes Gateway API standard implementation built directly on the battle-tested Envoy proxy engine. |
| **[Traefik Proxy](https://traefik.io/traefik/)** | MIT | Go | Modern HTTP reverse proxy and ingress controller with automatic service discovery (Docker, Swarm, Kubernetes, Consul) and ACME TLS. |
| **[Tyk Gateway (OSS)](https://github.com/TykTechnologies/tyk)** | MPL-2.0 | Go | Lightweight, blazing-fast open-source API gateway written in Go; supports GraphQL, gRPC, and REST with zero 3rd-party dependencies. |
