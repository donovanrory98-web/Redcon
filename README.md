export default function RedconWebsite() {
  const offers = [
    {
      title: "Weekend Rotisserie Club",
      price: "£25/week",
      description:
        "A ready-to-collect weekly chicken dinner bundle with simple add-ons and reliable repeat demand.",
      contents: ["1 rotisserie chicken", "2 sides", "Gravy or sauce"],
      why: "Perfect for busy households who want an easy weekly dinner sorted in advance.",
    },
    {
      title: "Weekly Butcher’s Box",
      price: "£40/week",
      description:
        "A core meat bundle built around convenience, value, and a dependable weekly shop habit.",
      contents: ["Chicken breasts", "Sausages", "Minced beef", "Steaks or roasting joint"],
      why: "Turns regular top-up customers into committed weekly subscribers.",
    },
    {
      title: "Friday Fish Club",
      price: "£35/week",
      description:
        "A weekly fish bundle that gives customers a simple Friday ritual and guaranteed collection.",
      contents: ["Fresh fillets", "Fishcakes or prawns", "Chef’s special"],
      why: "Ideal for repeat buying patterns and premium reserved products.",
    },
    {
      title: "Cheese & Wine Club",
      price: "£45/week",
      description:
        "A curated deli-style subscription with strong perceived value and easy gifting appeal.",
      contents: ["2 cheeses", "1 bottle of wine", "Crackers or chutney"],
      why: "Builds a high-margin recurring offer around discovery and indulgence.",
    },
  ];

  const benefits = [
    {
      title: "Predictable weekly revenue",
      text: "Bring in recurring income instead of relying only on one-off walk-in purchases.",
    },
    {
      title: "Higher basket size",
      text: "Bundle products together and give customers a reason to spend more each week.",
    },
    {
      title: "Simple setup",
      text: "Redcon helps you launch the offer, payment link, QR code posters, and landing page fast.",
    },
    {
      title: "No monthly fee",
      text: "You only pay when subscriptions generate revenue for your shop.",
    },
    {
      title: "No contract",
      text: "Keep it straightforward. No long tie-ins and no heavy commitment upfront.",
    },
    {
      title: "Your Stripe, your funds",
      text: "Customer payments go directly into your Stripe account. You stay in control.",
    },
  ];

  const faqs = [
    {
      q: "How long does setup take?",
      a: "Usually around 10–20 minutes. The setup is designed to be practical and lightweight, not a long software project.",
    },
    {
      q: "Do I need a new payment system?",
      a: "No. Redcon uses Stripe, so the merchant logs into or creates a Stripe account and payments go there directly.",
    },
    {
      q: "Who owns the customer payments?",
      a: "The merchant does. Funds go directly to the shop’s Stripe account, not to Redcon.",
    },
    {
      q: "Can customers cancel anytime?",
      a: "Yes. Customers can manage, update, pause, or cancel through Stripe’s subscription tools.",
    },
    {
      q: "Do I need to build a website?",
      a: "No. Redcon can help create a simple landing page and QR poster flow so customers can subscribe without you building anything complicated.",
    },
    {
      q: "What types of shops does this work for?",
      a: "It works best for independent butchers, fishmongers, delis, artisan food shops, wine and deli shops, and farm shops.",
    },
  ];

  return (
    <div className="min-h-screen bg-[#f7f1e8] text-[#171717] selection:bg-[#a12a2a] selection:text-white scroll-smooth">
      <style>{`
        html { scroll-behavior: smooth; }
        .grain {
          background-image:
            radial-gradient(circle at 20% 20%, rgba(161,42,42,0.06), transparent 22%),
            radial-gradient(circle at 80% 0%, rgba(0,0,0,0.04), transparent 18%),
            radial-gradient(circle at 0% 80%, rgba(201,166,107,0.08), transparent 20%);
        }
        .card-glow {
          box-shadow: 0 10px 35px rgba(0,0,0,0.07);
        }
        .soft-border {
          border: 1px solid rgba(23,23,23,0.08);
        }
      `}</style>

      <header className="sticky top-0 z-40 border-b border-black/5 bg-[#f7f1e8]/90 backdrop-blur">
        <div className="mx-auto flex max-w-7xl items-center justify-between px-5 py-4 sm:px-6 lg:px-8">
          <a href="#top" className="flex items-center gap-3">
            <div className="flex h-10 w-10 items-center justify-center rounded-2xl bg-[#a12a2a] text-lg font-semibold text-white shadow-sm">
              R
            </div>
            <div>
              <div className="text-lg font-semibold tracking-tight">Redcon</div>
              <div className="text-xs text-black/55">Subscription revenue for independent food shops</div>
            </div>
          </a>

          <nav className="hidden items-center gap-8 text-sm text-black/70 md:flex">
            <a href="#how-it-works" className="transition hover:text-black">How it works</a>
            <a href="#offers" className="transition hover:text-black">Examples</a>
            <a href="#pricing" className="transition hover:text-black">Pricing</a>
            <a href="#faq" className="transition hover:text-black">FAQ</a>
          </nav>

          <a
            href="#final-cta"
            className="rounded-full bg-[#171717] px-5 py-2.5 text-sm font-medium text-white transition hover:-translate-y-0.5 hover:bg-[#a12a2a]"
          >
            Book a quick demo
          </a>
        </div>
      </header>

      <main id="top">
        <section className="grain overflow-hidden">
          <div className="mx-auto grid max-w-7xl gap-12 px-5 py-16 sm:px-6 sm:py-20 lg:grid-cols-2 lg:px-8 lg:py-24">
            <div className="flex flex-col justify-center">
              <div className="mb-4 inline-flex w-fit items-center gap-2 rounded-full border border-[#a12a2a]/15 bg-white/70 px-3 py-1 text-sm text-[#7b2323]">
                <span className="h-2 w-2 rounded-full bg-[#a12a2a]" />
                Built for butchers, fishmongers, delis, and farm shops
              </div>

              <h1 className="max-w-2xl text-4xl font-semibold tracking-tight text-[#111111] sm:text-5xl lg:text-6xl">
                Turn regular customers into <span className="text-[#a12a2a]">weekly subscribers</span>
              </h1>

              <p className="mt-6 max-w-xl text-lg leading-8 text-black/70">
                Redcon helps independent food shops launch simple subscription bundles in around 10–20 minutes. Payments go directly to your Stripe account. No setup fee. No monthly fee. No contract.
              </p>

              <div className="mt-8 flex flex-col gap-3 sm:flex-row">
                <a
                  href="#final-cta"
                  className="rounded-full bg-[#a12a2a] px-6 py-3 text-center text-sm font-semibold text-white transition hover:-translate-y-0.5 hover:shadow-lg"
                >
                  See how it could work for your shop
                </a>
                <a
                  href="#how-it-works"
                  className="rounded-full border border-black/10 bg-white/80 px-6 py-3 text-center text-sm font-semibold text-[#171717] transition hover:-translate-y-0.5 hover:bg-white"
                >
                  How Redcon works
                </a>
              </div>

              <div className="mt-8 grid max-w-xl grid-cols-1 gap-3 text-sm text-black/65 sm:grid-cols-3">
                <div className="rounded-2xl border border-black/5 bg-white/70 px-4 py-3">Setup takes about 10–20 minutes</div>
                <div className="rounded-2xl border border-black/5 bg-white/70 px-4 py-3">Stripe payments go directly to you</div>
                <div className="rounded-2xl border border-black/5 bg-white/70 px-4 py-3">You only pay 7.5% of subscription revenue</div>
              </div>
            </div>

            <div className="relative">
              <div className="card-glow relative rounded-[2rem] border border-black/5 bg-white p-5 sm:p-6">
                <div className="mb-5 flex items-center justify-between">
                  <div>
                    <div className="text-sm text-black/50">Example shop setup</div>
                    <div className="text-2xl font-semibold">Kola Butchers</div>
                  </div>
                  <div className="rounded-full bg-[#f7f1e8] px-3 py-1 text-sm font-medium text-[#7b2323]">
                    Live in under 20 mins
                  </div>
                </div>

                <div className="grid gap-4">
                  <div className="rounded-3xl bg-[#fcfaf6] p-5 soft-border">
                    <div className="flex items-start justify-between gap-4">
                      <div>
                        <div className="text-sm text-black/50">Subscription offer</div>
                        <div className="mt-1 text-xl font-semibold">Weekly Butcher’s Box</div>
                        <div className="mt-1 text-black/60">£40 per week · Collection every Saturday</div>
                      </div>
                      <div className="rounded-2xl bg-[#171717] px-3 py-2 text-sm font-semibold text-white">Stripe link ready</div>
                    </div>

                    <div className="mt-4 grid grid-cols-2 gap-3 text-sm text-black/70">
                      <div className="rounded-2xl bg-white px-4 py-3 soft-border">Chicken breasts</div>
                      <div className="rounded-2xl bg-white px-4 py-3 soft-border">Sausages</div>
                      <div className="rounded-2xl bg-white px-4 py-3 soft-border">Minced beef</div>
                      <div className="rounded-2xl bg-white px-4 py-3 soft-border">Weekend roasting cut</div>
                    </div>
                  </div>

                  <div className="grid gap-4 sm:grid-cols-[1fr_220px]">
                    <div className="rounded-3xl bg-[#171717] p-5 text-white">
                      <div className="text-sm text-white/60">Merchant view</div>
                      <div className="mt-3 grid gap-3">
                        <div className="rounded-2xl bg-white/8 px-4 py-3">
                          <div className="text-xs text-white/60">Active subscribers</div>
                          <div className="text-2xl font-semibold">37</div>
                        </div>
                        <div className="rounded-2xl bg-white/8 px-4 py-3">
                          <div className="text-xs text-white/60">This week’s collections</div>
                          <div className="text-2xl font-semibold">34</div>
                        </div>
                        <div className="rounded-2xl bg-white/8 px-4 py-3">
                          <div className="text-xs text-white/60">Paused or cancelled</div>
                          <div className="text-2xl font-semibold">3</div>
                        </div>
                      </div>
                    </div>

                    <div className="rounded-3xl border border-dashed border-[#a12a2a]/25 bg-[#fffdf9] p-5">
                      <div className="text-sm text-black/50">In-store poster</div>
                      <div className="mt-4 rounded-[1.5rem] bg-[#a12a2a] p-4 text-white">
                        <div className="text-sm text-white/80">Scan to subscribe</div>
                        <div className="mt-2 text-lg font-semibold">Weekly Roast Club</div>
                        <div className="mt-1 text-sm text-white/80">Reserve your weekend bundle</div>
                        <div className="mt-4 grid grid-cols-4 gap-1 rounded-xl bg-white p-2">
                          {Array.from({ length: 16 }).map((_, i) => (
                            <div key={i} className={`aspect-square rounded-sm ${i % 3 === 0 ? 'bg-black' : 'bg-black/15'}`} />
                          ))}
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              <div className="absolute -bottom-5 -left-3 hidden rounded-2xl border border-black/5 bg-white px-4 py-3 text-sm text-black/60 shadow-md sm:block">
                Customers subscribe by QR code or landing page
              </div>
            </div>
          </div>
        </section>

        <section id="how-it-works" className="mx-auto max-w-7xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
          <div className="max-w-2xl">
            <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">How it works</div>
            <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
              Launch a weekly subscription bundle without turning your shop into a software project
            </h2>
            <p className="mt-4 text-lg text-black/70">
              The setup is practical and fast. Redcon helps structure the offer, connect Stripe, create the checkout flow, and get customers subscribing.
            </p>
          </div>

          <div className="mt-12 grid gap-4 md:grid-cols-5">
            {[
              ["1", "Create your offer", "Choose the bundle, collection day, and weekly price."],
              ["2", "Connect Stripe", "Log into or create your Stripe account so payments go directly to you."],
              ["3", "Launch checkout and QR posters", "Redcon sets up the payment link, landing page, and in-store QR poster."],
              ["4", "Customers subscribe", "They scan, subscribe through Stripe, and receive confirmation by email."],
              ["5", "Prepare and collect weekly", "You see who is active, what needs preparing, and who is collecting."],
            ].map(([num, title, text]) => (
              <div key={num} className="card-glow rounded-[1.75rem] bg-white p-5 soft-border transition hover:-translate-y-1">
                <div className="flex h-10 w-10 items-center justify-center rounded-2xl bg-[#a12a2a] text-sm font-semibold text-white">
                  {num}
                </div>
                <h3 className="mt-4 text-lg font-semibold">{title}</h3>
                <p className="mt-2 text-sm leading-6 text-black/65">{text}</p>
              </div>
            ))}
          </div>
        </section>

        <section className="border-y border-black/5 bg-white/60">
          <div className="mx-auto max-w-7xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
            <div className="max-w-2xl">
              <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">Why merchants use it</div>
              <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
                Built to make recurring revenue feel simple, not technical
              </h2>
            </div>

            <div className="mt-12 grid gap-4 sm:grid-cols-2 lg:grid-cols-3">
              {benefits.map((item) => (
                <div key={item.title} className="rounded-[1.75rem] bg-white p-6 soft-border transition hover:-translate-y-1 hover:shadow-lg">
                  <h3 className="text-xl font-semibold tracking-tight">{item.title}</h3>
                  <p className="mt-3 text-sm leading-6 text-black/65">{item.text}</p>
                </div>
              ))}
            </div>
          </div>
        </section>

        <section id="offers" className="mx-auto max-w-7xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
          <div className="flex flex-col gap-4 lg:flex-row lg:items-end lg:justify-between">
            <div className="max-w-2xl">
              <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">Example subscription offers</div>
              <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
                Real offers independent food shops can launch
              </h2>
            </div>
            <p className="max-w-xl text-black/68">
              The best offers are clear, repeatable, and easy to collect. They fit buying habits customers already have.
            </p>
          </div>

          <div className="mt-12 grid gap-5 lg:grid-cols-2">
            {offers.map((offer) => (
              <div key={offer.title} className="card-glow rounded-[2rem] bg-white p-6 soft-border transition hover:-translate-y-1">
                <div className="flex flex-col gap-4 sm:flex-row sm:items-start sm:justify-between">
                  <div>
                    <div className="text-sm text-black/50">Subscription example</div>
                    <h3 className="mt-1 text-2xl font-semibold tracking-tight">{offer.title}</h3>
                    <p className="mt-2 text-black/65">{offer.description}</p>
                  </div>
                  <div className="rounded-full bg-[#171717] px-4 py-2 text-sm font-semibold text-white">
                    {offer.price}
                  </div>
                </div>

                <div className="mt-5 grid gap-4 md:grid-cols-2">
                  <div className="rounded-3xl bg-[#fcfaf6] p-5 soft-border">
                    <div className="text-sm font-semibold text-black">Example contents</div>
                    <ul className="mt-3 space-y-2 text-sm text-black/70">
                      {offer.contents.map((item) => (
                        <li key={item} className="flex items-start gap-2">
                          <span className="mt-1 h-1.5 w-1.5 rounded-full bg-[#a12a2a]" />
                          <span>{item}</span>
                        </li>
                      ))}
                    </ul>
                  </div>
                  <div className="rounded-3xl bg-[#f7f1e8] p-5 soft-border">
                    <div className="text-sm font-semibold text-black">Why customers subscribe</div>
                    <p className="mt-3 text-sm leading-6 text-black/70">{offer.why}</p>
                  </div>
                </div>
              </div>
            ))}
          </div>
        </section>

        <section id="pricing" className="bg-[#171717] text-white">
          <div className="mx-auto grid max-w-7xl gap-8 px-5 py-16 sm:px-6 lg:grid-cols-[1.1fr_0.9fr] lg:px-8 lg:py-24">
            <div>
              <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#e1b78d]">Pricing</div>
              <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
                7.5% of subscription revenue only
              </h2>
              <p className="mt-4 max-w-2xl text-lg text-white/72">
                No setup fee. No monthly software fee. No contract. Redcon only earns money when your shop earns money.
              </p>

              <div className="mt-8 grid max-w-2xl gap-3 sm:grid-cols-2">
                {["No setup fee", "No monthly fee", "No long contract", "Merchant keeps Stripe account and funds"].map((item) => (
                  <div key={item} className="rounded-2xl border border-white/10 bg-white/5 px-4 py-3 text-sm text-white/82">
                    {item}
                  </div>
                ))}
              </div>
            </div>

            <div className="rounded-[2rem] border border-white/10 bg-white/6 p-6 backdrop-blur">
              <div className="text-sm text-white/60">Worked example</div>
              <div className="mt-4 rounded-3xl bg-white text-[#171717] p-6">
                <div className="text-sm text-black/55">Monthly subscription revenue</div>
                <div className="mt-1 text-4xl font-semibold">£2,000</div>

                <div className="my-5 h-px bg-black/10" />

                <div className="flex items-center justify-between text-sm">
                  <span className="text-black/60">Redcon fee</span>
                  <span className="font-semibold">7.5%</span>
                </div>

                <div className="mt-3 flex items-center justify-between text-lg">
                  <span className="text-black/70">Redcon earns</span>
                  <span className="font-semibold text-[#a12a2a]">£150</span>
                </div>

                <p className="mt-5 text-sm leading-6 text-black/65">
                  Simple commercial terms. Easy to understand. Easy to explain. Easy to trial.
                </p>
              </div>
            </div>
          </div>
        </section>

        <section className="mx-auto max-w-7xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
          <div className="grid gap-10 lg:grid-cols-[0.95fr_1.05fr] lg:items-center">
            <div>
              <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">Merchant dashboard and operations</div>
              <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
                See what needs preparing each week without digging through admin
              </h2>
              <p className="mt-4 text-lg text-black/70">
                Redcon is designed to keep the operational side clear. The merchant can see active subscribers, weekly orders, paused or cancelled customers, and a practical collection list.
              </p>

              <div className="mt-8 grid gap-3">
                {[
                  "Active subscribers at a glance",
                  "Weekly orders to prepare",
                  "Paused and cancelled customers clearly marked",
                  "Simple collection list for the counter or prep area",
                ].map((item) => (
                  <div key={item} className="rounded-2xl border border-black/8 bg-white px-4 py-3 text-sm text-black/72 shadow-sm">
                    {item}
                  </div>
                ))}
              </div>
            </div>

            <div className="card-glow rounded-[2rem] bg-white p-5 soft-border sm:p-6">
              <div className="flex items-center justify-between border-b border-black/8 pb-4">
                <div>
                  <div className="text-sm text-black/50">Mock dashboard</div>
                  <div className="text-xl font-semibold">Weekly collections overview</div>
                </div>
                <div className="rounded-full bg-[#f7f1e8] px-3 py-1 text-sm text-[#7b2323]">Saturday collection</div>
              </div>

              <div className="mt-5 grid gap-4 md:grid-cols-3">
                {[
                  ["42", "Active subscribers"],
                  ["39", "Orders due this week"],
                  ["3", "Paused / cancelled"],
                ].map(([num, label]) => (
                  <div key={label} className="rounded-3xl bg-[#fcfaf6] p-5 soft-border">
                    <div className="text-3xl font-semibold">{num}</div>
                    <div className="mt-1 text-sm text-black/55">{label}</div>
                  </div>
                ))}
              </div>

              <div className="mt-5 overflow-hidden rounded-3xl border border-black/8">
                <div className="grid grid-cols-[1.2fr_1fr_1fr] bg-[#171717] px-4 py-3 text-sm font-medium text-white">
                  <div>Customer</div>
                  <div>Offer</div>
                  <div>Status</div>
                </div>
                {[
                  ["Anna M.", "Butcher’s Box", "Collecting"],
                  ["James T.", "Rotisserie Club", "Collecting"],
                  ["Priya S.", "Fish Club", "Paused"],
                  ["Oliver B.", "Butcher’s Box", "Collecting"],
                ].map((row, idx) => (
                  <div key={idx} className="grid grid-cols-[1.2fr_1fr_1fr] border-t border-black/6 bg-white px-4 py-3 text-sm text-black/70">
                    <div>{row[0]}</div>
                    <div>{row[1]}</div>
                    <div>
                      <span className={`rounded-full px-2.5 py-1 text-xs font-medium ${row[2] === 'Paused' ? 'bg-black/8 text-black/60' : 'bg-[#a12a2a]/10 text-[#7b2323]'}`}>
                        {row[2]}
                      </span>
                    </div>
                  </div>
                ))}
              </div>
            </div>
          </div>
        </section>

        <section className="border-y border-black/5 bg-white/60">
          <div className="mx-auto max-w-7xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
            <div className="max-w-2xl">
              <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">Why this works for food shops</div>
              <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
                Subscription bundles fit the way people already buy food
              </h2>
            </div>

            <div className="mt-12 grid gap-5 lg:grid-cols-4">
              {[
                {
                  title: "Repeat buying behaviour",
                  text: "Customers already come back for the same core items each week. A subscription simply makes that habit easier and more consistent.",
                },
                {
                  title: "Weekend rituals",
                  text: "Roast dinners, Friday fish, chicken night, deli treats, and wine weekends naturally suit a weekly recurring offer.",
                },
                {
                  title: "Reserved products",
                  text: "Customers like the confidence of knowing their bundle is set aside and ready for collection.",
                },
                {
                  title: "Convenience and value",
                  text: "A clear bundle removes friction, raises spend, and gives customers a reason to stay loyal to one shop.",
                },
              ].map((item) => (
                <div key={item.title} className="rounded-[1.75rem] bg-[#f7f1e8] p-6 soft-border">
                  <h3 className="text-xl font-semibold tracking-tight">{item.title}</h3>
                  <p className="mt-3 text-sm leading-6 text-black/68">{item.text}</p>
                </div>
              ))}
            </div>
          </div>
        </section>

        <section id="faq" className="mx-auto max-w-5xl px-5 py-16 sm:px-6 lg:px-8 lg:py-24">
          <div className="text-center">
            <div className="text-sm font-semibold uppercase tracking-[0.22em] text-[#a12a2a]">FAQ</div>
            <h2 className="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">
              Clear answers for independent shops
            </h2>
          </div>

          <div className="mt-12 grid gap-4">
            {faqs.map((faq) => (
              <details key={faq.q} className="group rounded-[1.5rem] bg-white p-6 soft-border open:shadow-md">
                <summary className="flex cursor-pointer list-none items-center justify-between gap-4 text-left text-lg font-semibold">
                  <span>{faq.q}</span>
                  <span className="rounded-full border border-black/10 px-3 py-1 text-sm text-black/45 transition group-open:rotate-45">+</span>
                </summary>
                <p className="mt-4 max-w-3xl text-sm leading-7 text-black/68">{faq.a}</p>
              </details>
            ))}
          </div>
        </section>

        <section id="final-cta" className="px-5 pb-16 sm:px-6 lg:px-8 lg:pb-24">
          <div className="mx-auto max-w-6xl overflow-hidden rounded-[2.5rem] bg-[#a12a2a] text-white card-glow">
            <div className="grid gap-8 px-6 py-10 sm:px-8 lg:grid-cols-[1.05fr_0.95fr] lg:px-12 lg:py-14">
              <div>
                <div className="text-sm font-semibold uppercase tracking-[0.22em] text-white/75">Launch your first offer</div>
                <h2 className="mt-3 max-w-2xl text-3xl font-semibold tracking-tight sm:text-4xl">
                  See how Redcon could work for your shop
                </h2>
                <p className="mt-4 max-w-xl text-white/85">
                  Launch a simple weekly subscription bundle, keep payments flowing directly to your Stripe account, and start building recurring revenue without adding complicated software.
                </p>

                <div className="mt-6 flex flex-wrap gap-3 text-sm text-white/82">
                  <div className="rounded-full border border-white/15 bg-white/10 px-3 py-2">10–20 minute setup</div>
                  <div className="rounded-full border border-white/15 bg-white/10 px-3 py-2">No setup fee</div>
                  <div className="rounded-full border border-white/15 bg-white/10 px-3 py-2">7.5% only when you sell</div>
                </div>
              </div>

              <div className="rounded-[2rem] bg-white p-5 text-[#171717] sm:p-6">
                <div className="text-sm text-black/50">Express interest</div>
                <form className="mt-4 grid gap-3">
                  <input
                    type="text"
                    placeholder="Shop name"
                    className="rounded-2xl border border-black/10 bg-[#fcfaf6] px-4 py-3 text-sm outline-none transition focus:border-[#a12a2a]"
                  />
                  <input
                    type="text"
                    placeholder="Your name"
                    className="rounded-2xl border border-black/10 bg-[#fcfaf6] px-4 py-3 text-sm outline-none transition focus:border-[#a12a2a]"
                  />
                  <input
                    type="email"
                    placeholder="Email address"
                    className="rounded-2xl border border-black/10 bg-[#fcfaf6] px-4 py-3 text-sm outline-none transition focus:border-[#a12a2a]"
                  />
                  <select className="rounded-2xl border border-black/10 bg-[#fcfaf6] px-4 py-3 text-sm outline-none transition focus:border-[#a12a2a]">
                    <option>Shop type</option>
                    <option>Butcher</option>
                    <option>Fishmonger</option>
                    <option>Deli</option>
                    <option>Farm shop</option>
                    <option>Wine and deli shop</option>
                    <option>Other artisan food shop</option>
                  </select>
                  <textarea
                    rows={4}
                    placeholder="What kind of subscription offer are you thinking about?"
                    className="rounded-2xl border border-black/10 bg-[#fcfaf6] px-4 py-3 text-sm outline-none transition focus:border-[#a12a2a]"
                  />
                  <button
                    type="button"
                    className="mt-2 rounded-full bg-[#171717] px-6 py-3 text-sm font-semibold text-white transition hover:-translate-y-0.5 hover:bg-black"
                  >
                    Book a quick demo
                  </button>
                </form>
                <p className="mt-4 text-xs leading-5 text-black/50">
                  Placeholder form. Connect this to your email tool, form handler, or CRM when you deploy.
                </p>
              </div>
            </div>
          </div>
        </section>
      </main>
    </div>
  );
}
