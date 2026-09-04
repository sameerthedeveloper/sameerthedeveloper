{/* PROFILE — from GitHub README, styled to match existing sections */}
<section id="profile" className="flex min-h-svh scroll-mt-24 flex-col justify-center px-5 py-24 sm:px-8">
  <div className="mx-auto grid max-w-wide gap-10 lg:grid-cols-[1fr_1.7fr] lg:gap-16">
    <div className="lg:sticky lg:top-28 lg:self-start">
      <SplitHeading
        text="Right now."
        className="text-4xl font-semibold tracking-tight text-ink sm:text-5xl"
      />
      <p className="reveal mt-4 max-w-xs text-muted">
        BTech CSE (3rd yr) — shipping production web apps, React/Next.js frontend, Firebase/Supabase backend.
      </p>
    </div>

    <div className="flex flex-col gap-10">
      <ol className="border-t border-line">
        {[
          { label: 'Building', value: 'JARVIS — local voice assistant (Electron, Vosk, Ollama, Piper TTS)' },
          { label: 'Learning', value: 'System design · DBMS internals · OS fundamentals' },
          { label: 'Goal', value: 'Frontend/full-stack internship — remote / Chennai' },
          { label: 'Approach', value: 'Halal-first in fintech & dev work' },
        ].map((item, i) => (
          <li key={item.label} className="reveal service-row group relative border-b border-line py-6">
            <span className="service-row-bar pointer-events-none absolute -left-5 top-0 bottom-0 w-0.75 origin-center scale-y-0 bg-accent transition-transform duration-300 ease-out group-hover:scale-y-100 sm:-left-6" />
            <div className="flex items-baseline gap-4 sm:gap-6">
              <span className="font-mono text-sm text-faint transition-colors duration-300 group-hover:text-accent">
                {String(i + 1).padStart(2, '0')}
              </span>
              <div className="min-w-0 flex-1">
                <h3 className="text-lg font-medium text-ink transition-colors duration-300 group-hover:text-accent">
                  {item.label}
                </h3>
                <p className="mt-1 text-[15px] text-muted">{item.value}</p>
              </div>
            </div>
          </li>
        ))}
      </ol>

      <div className="reveal">
        <p className="mb-4 text-sm text-muted">Stack</p>
        <div className="flex flex-wrap gap-2">
          {['HTML', 'CSS', 'JS', 'TS', 'React', 'Next.js', 'Tailwind', 'Firebase', 'Supabase', 'Python', 'FastAPI', 'Git'].map((tech) => (
            <span
              key={tech}
              className="rounded-full border border-line px-3 py-1 text-xs font-medium text-muted transition-colors hover:border-accent hover:text-accent"
            >
              {tech}
            </span>
          ))}
        </div>
      </div>

      <div className="reveal">
        <p className="text-sm text-muted">
          Honest, clean code. Build useful things. Halal-first in fintech/dev work. Daily commits.
        </p>
        <p className="mt-2 text-xs text-faint">Knowledge is amanah. Use it right.</p>
      </div>
    </div>
  </div>
</section>
