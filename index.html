import React, { useMemo, useState } from "react";

const questions = [
  {
    id: 1,
    question: "In welk land werd Napoleon Bonaparte geboren?",
    answers: ["frankrijk", "corsica", "frankrijk (corsica)", "corsica (frankrijk)"],
    correctLabel: "Frankrijk / Corsica",
    feedback:
      "Napoleon werd geboren op Corsica. Dat eiland was kort daarvoor Frans geworden. Daarom zijn zowel ‘Corsica’ als ‘Frankrijk’ meestal goed te rekenen.",
  },
  {
    id: 2,
    question:
      "Welke belangrijke militaire overwinning behaalde Napoleon in 1805 tegen Oostenrijk en Rusland?",
    answers: ["slag bij austerlitz", "austerlitz"],
    correctLabel: "Slag bij Austerlitz",
    feedback:
      "De Slag bij Austerlitz was een van Napoleons grootste overwinningen. Deze slag staat ook bekend als de Slag der Drie Keizers.",
  },
  {
    id: 3,
    question: "Wat was de naam van het wetboek dat Napoleon invoerde?",
    answers: ["code napoléon", "code napoleon", "burgerlijk wetboek"],
    correctLabel: "Code Napoléon / Burgerlijk Wetboek",
    feedback:
      "De Code Napoléon werd een invloedrijk wetboek in Europa. Ook ‘Burgerlijk Wetboek’ is hier een goed antwoord.",
  },
  {
    id: 4,
    question: "Naar welk eiland werd Napoleon voor het eerst verbannen?",
    answers: ["elba"],
    correctLabel: "Elba",
    feedback:
      "Napoleon werd in 1814 verbannen naar Elba. Later keerde hij nog kort terug aan de macht.",
  },
  {
    id: 5,
    question: "In welk jaar vond de Slag bij Waterloo plaats?",
    answers: ["1815"],
    correctLabel: "1815",
    feedback:
      "De Slag bij Waterloo vond plaats in 1815 en betekende Napoleons definitieve nederlaag.",
  },
];

export default function NapoleonQuizApp() {
  const [answers, setAnswers] = useState(() =>
    Object.fromEntries(questions.map((q) => [q.id, ""]))
  );
  const [checked, setChecked] = useState(false);

  const results = useMemo(() => {
    return questions.map((q) => {
      const raw = answers[q.id] ?? "";
      const normalized = raw.trim().toLowerCase();
      const correct = q.answers.includes(normalized);
      return { ...q, userAnswer: raw, correct };
    });
  }, [answers]);

  const score = results.filter((r) => r.correct).length;

  function handleChange(id, value) {
    setAnswers((prev) => ({ ...prev, [id]: value }));
  }

  function handleCheck() {
    setChecked(true);
  }

  function handleReset() {
    setAnswers(Object.fromEntries(questions.map((q) => [q.id, ""])));
    setChecked(false);
  }

  function getScoreText(currentScore) {
    if (currentScore === 5) return "Uitstekend";
    if (currentScore === 4) return "Goed";
    if (currentScore === 3) return "Voldoende";
    return "Nog even oefenen";
  }

  return (
    <div className="min-h-screen bg-white p-6 md:p-10">
      <div className="mx-auto max-w-3xl rounded-3xl border border-slate-200 bg-white p-6 shadow-sm md:p-8">
        <h1 className="text-3xl font-bold tracking-tight">Quiz over Napoleon</h1>
        <p className="mt-3 text-base text-slate-700">
          Beantwoord de 5 vragen en klik daarna op <strong>Controleer antwoorden</strong>.
          Je krijgt per vraag feedback te zien.
        </p>

        <div className="mt-8 space-y-6">
          {results.map((result, index) => (
            <div key={result.id} className="rounded-2xl border border-slate-200 p-5">
              <label className="block text-base font-semibold text-slate-900">
                {index + 1}. {result.question}
              </label>

              <input
                type="text"
                value={answers[result.id]}
                onChange={(e) => handleChange(result.id, e.target.value)}
                className="mt-3 w-full rounded-xl border border-slate-300 px-4 py-3 text-base outline-none focus:border-slate-500"
                placeholder="Typ je antwoord hier"
              />

              {checked && (
                <div
                  className={`mt-4 rounded-xl p-4 text-sm leading-6 ${
                    result.correct
                      ? "border border-green-200 bg-green-50 text-green-900"
                      : "border border-red-200 bg-red-50 text-red-900"
                  }`}
                >
                  <p className="font-semibold">
                    {result.correct ? "Goed antwoord" : "Niet goed"}
                  </p>

                  {!result.correct && (
                    <p className="mt-1">
                      <strong>Juiste antwoord:</strong> {result.correctLabel}
                    </p>
                  )}

                  <p className="mt-1">{result.feedback}</p>
                </div>
              )}
            </div>
          ))}
        </div>

        <div className="mt-8 flex flex-wrap gap-3">
          <button
            onClick={handleCheck}
            className="rounded-2xl bg-slate-900 px-5 py-3 text-white transition hover:opacity-90"
          >
            Controleer antwoorden
          </button>
          <button
            onClick={handleReset}
            className="rounded-2xl border border-slate-300 px-5 py-3 text-slate-800 transition hover:bg-slate-50"
          >
            Opnieuw beginnen
          </button>
        </div>

        {checked && (
          <div className="mt-8 rounded-2xl border border-slate-200 bg-slate-50 p-5">
            <h2 className="text-xl font-semibold">Jouw score</h2>
            <p className="mt-2 text-base text-slate-800">
              Je hebt <strong>{score} van de 5</strong> vragen goed.
            </p>
            <p className="mt-1 text-slate-700">Beoordeling: {getScoreText(score)}</p>
          </div>
        )}
      </div>
    </div>
  );
}
