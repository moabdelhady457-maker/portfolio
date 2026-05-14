# portfolioexport default function Portfolio() {
  const projects = [
    {
      title: "Design Optimization of Hydraulic Press Plate",
      desc: "Finite Element Analysis project focused on optimization, material reduction, and cost effectiveness.",
    },
    {
      title: "Hydro-pneumatic Suspension System",
      desc: "Mathematical modeling and sensitivity analysis for vehicle suspension performance.",
    },
    {
      title: "Disk Brake Rotor Thermal Analysis",
      desc: "Thermal simulation and analysis using ANSYS Workbench with real-world conditions.",
    },
    {
      title: "Exhaust System & Muffler Design",
      desc: "CFD and acoustic analysis for optimized exhaust gas flow and noise reduction.",
    },
  ];

  const skills = [
    "AutoCAD",
    "CATIA V5",
    "ANSYS",
    "MATLAB",
    "FEA",
    "CFD",
    "Modeling & Simulation",
    "Optimization",
  ];

  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center px-6 py-24 bg-gradient-to-b from-zinc-900 to-black">
        <div className="w-36 h-36 rounded-full border-4 border-cyan-400 overflow-hidden shadow-2xl mb-6">
          <img
            src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop"
            alt="profile"
            className="w-full h-full object-cover"
          />
        </div>

        <h1 className="text-5xl md:text-6xl font-bold tracking-wide">
          Mohamed Sayed Abdelhady
        </h1>

        <p className="mt-4 text-zinc-300 text-lg md:text-xl max-w-2xl leading-relaxed">
          Engineering Student passionate about Product Development, CAD/CAE,
          Finite Element Analysis, Simulation, and Automotive Design.
        </p>

        <div className="flex gap-4 mt-8 flex-wrap justify-center">
          <a
            href="#projects"
            className="px-6 py-3 rounded-2xl bg-cyan-500 hover:bg-cyan-400 transition text-black font-semibold"
          >
            View Projects
          </a>

          <a
            href="/Mohamed_Sayed_CV.pdf"
            className="px-6 py-3 rounded-2xl border border-zinc-700 hover:border-cyan-400 transition"
          >
            Download CV
          </a>
        </div>
      </section>

      {/* About */}
      <section className="max-w-6xl mx-auto px-6 py-20">
        <h2 className="text-4xl font-bold mb-8 text-cyan-400">About Me</h2>

        <div className="bg-zinc-900 rounded-3xl p-8 shadow-xl border border-zinc-800 leading-8 text-zinc-300 text-lg">
          I am an engineering student at Cairo Higher Institute with strong
          interest in product development, simulation, CAD/CAE design, and
          optimization techniques. I enjoy solving engineering problems through
          analytical thinking, simulations, and real-world design applications.
        </div>
      </section>

      {/* Skills */}
      <section className="max-w-6xl mx-auto px-6 py-10">
        <h2 className="text-4xl font-bold mb-8 text-cyan-400">Skills</h2>

        <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
          {skills.map((skill, index) => (
            <div
              key={index}
              className="bg-zinc-900 border border-zinc-800 rounded-2xl p-5 text-center hover:border-cyan-400 transition"
            >
              {skill}
            </div>
          ))}
        </div>
      </section>

      {/* Projects */}
      <section id="projects" className="max-w-6xl mx-auto px-6 py-20">
        <h2 className="text-4xl font-bold mb-10 text-cyan-400">Projects</h2>

        <div className="grid md:grid-cols-2 gap-8">
          {projects.map((project, index) => (
            <div
              key={index}
              className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 hover:border-cyan-400 transition shadow-xl"
            >
              <h3 className="text-2xl font-semibold mb-4">{project.title}</h3>
              <p className="text-zinc-400 leading-7">{project.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Experience */}
      <section className="max-w-6xl mx-auto px-6 py-10">
        <h2 className="text-4xl font-bold mb-8 text-cyan-400">Experience & Training</h2>

        <div className="space-y-6">
          <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-6">
            <h3 className="text-2xl font-semibold mb-2">
              Automotive Industry Simulation Internship
            </h3>
            <p className="text-zinc-400">Expertshub, Pune — June 2022</p>
          </div>

          <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-6">
            <h3 className="text-2xl font-semibold mb-2">
              Machining & Quality Control Training
            </h3>
            <p className="text-zinc-400">Amul Group of Industries — February 2022</p>
          </div>
        </div>
      </section>

      {/* Contact */}
      <section className="max-w-6xl mx-auto px-6 py-20">
        <div className="bg-gradient-to-r from-cyan-500/20 to-zinc-900 border border-cyan-500/20 rounded-3xl p-10 text-center">
          <h2 className="text-4xl font-bold mb-4">Contact Me</h2>

          <p className="text-zinc-300 text-lg mb-6">
            Let's connect and build something amazing.
          </p>

          <div className="flex flex-col gap-3 text-lg text-zinc-200">
            <span>📧 moabdelhady457@gmail.com</span>
            <span>📱 +20 01014955516</span>
            <span>📍 Cairo, Egypt</span>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-zinc-800 py-8 text-center text-zinc-500">
        © 2026 Mohamed Sayed Abdelhady. All Rights Reserved.
      </footer>
    </div>
  );
}
