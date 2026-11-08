# Awesome-API-Gateway-Routing-Management

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag the data and category problems before you publish this.

## The category problem

**"Postman Gateway"** does not exist as a product. Postman is an API client and collaboration platform; its pricing starts at $12/user/month for the client . It has no gateway product to list alongside Kong, Traefik, or APISIX. **Remove it or reframe it as an API client, not a gateway.**

**Traefik** is an open-source reverse proxy and ingress controller under MIT, with commercial Hub tiers gated behind a sales contact form and a 30-day trial . It is a legitimate gateway but sits in a different class from full API management platforms.

**NGINX Plus** is proprietary (CDW lists one instance at $6,468.99 for a subscription license plus support) . NGINX Open Source is free, but it is a web server and reverse proxy, not a full API management platform. Listing "NGINX Plus" without distinguishing OSS from Plus will confuse readers.

## What the search results actually contain

**Pricing (usable):**
- **Tyk**: Gateway and Pump are **MPL 2.0 free**; Dashboard, Developer Portal, Operator, and MDCB require a license. **No public list prices**—Core is usage-based by APIs managed; Professional is architecture-based by data planes, environments, and control planes. **Tyk Hybrid** runs gateways in your cluster with Tyk Cloud hosting the control plane . Tyk benchmarks at **~68,000 req/s at 1.7ms p99** on AWS c5.4xlarge with encrypted API-key auth, versus Kong's ~24,000 at 4.3ms .
- **Azure API Management**: China region pricing shows **Developer tier ~¥373.64/month, Basic ~¥1,144.72/month, Standard ~¥5,341.47/month, Premium ~¥21,741.84/month** .
- **Apigee**: **Pay-as-you-go** introduced as a complement to subscription plans; 60-day free evaluation. Charged on gateway nodes per minute, API analytics per request, and networking usage .
- **AWS API Gateway**: Pay-per-use, no upfront commitment; HTTP APIs charged per million requests with volume tiers (first 300M at $1.00/million, next 132M at $0.90/million in the Arabic pricing example) .
- **Traefik**: Proxy is **MIT free**; commercial Hub tiers gated behind sales contact; 30-day trial for API Gateway tier .
- **NGINX Plus**: CDW lists $6,468.99 for a 1-month subscription license plus standard support for one instance .

**Open-source licenses (usable):**
- **Apache APISIX**: **Apache 2.0**; built on NGINX + LuaJIT; etcd-backed dynamic config or standalone file-based; Admin API; plugin languages include Lua, Java, Go, Python, Wasm .
- **Kong Gateway OSS**: **Apache 2.0**; NGINX + LuaJIT; PostgreSQL-backed, DB-less, or hybrid modes .
- **Envoy Gateway**: **Apache 2.0** (Envoy itself); xDS-based dynamic config; C++ core with Wasm filters .
- **Traefik Proxy**: **MIT**; Go-based; provider integrations for Docker/Kubernetes/Consul; ACME certificate resolver .

**What is missing:**
- **No star counts** for any of these repos.
- **No revenue or valuation data** for any vendor.
- **No pricing** for Kong Konnect, Postman (beyond $12/user/month client pricing), or Envoy Gateway (it is free OSS).
- **No confirmation** that "Postman Gateway" exists.

## What I recommend

**Split the list into three honest categories:**

**1. Full API Management Platforms** (proprietary or open-core): Kong, Apigee, Azure API Management, Tyk (Core/Professional), WSO2 (if you add it).

**2. Open-Source Gateways** (genuinely free): **Apache APISIX** (Apache 2.0), **Kong Gateway OSS** (Apache 2.0), **Envoy Gateway** (Apache 2.0), **Traefik Proxy** (MIT), **Tyk Gateway** (MPL 2.0). This section is strong and well-supported by the results.

**3. Outliers to remove or reframe:** Postman (not a gateway); NGINX Plus (proprietary web server/reverse proxy, not full APIM).

**The open-source section is genuinely strong**—APISIX, Kong OSS, Envoy, Traefik, and Tyk Gateway all have clear licenses and active projects. The proprietary section has usable pricing for Azure, Apigee, AWS, Tyk, Traefik Hub, and NGINX Plus.

If you paste your current `README.md` and confirm you want the split framing, I will produce the complete file as text for you to save. I will not list Postman as a gateway, fabricate star counts, or invent pricing for Kong Konnect or Envoy Gateway that the results do not support.
