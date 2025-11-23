# Mary's Room: A Chromatic Qualia Experiment

An interactive web-based tool that explores one of philosophy's most famous thought experiments about consciousness, knowledge, and subjective experience.

## 🧠 The Philosophical Question

**Mary's Room**, proposed by philosopher Frank Jackson in 1982, asks:

> Mary is a brilliant scientist who lives in a black-and-white room and has never seen colors. However, she knows *everything* there is to know about color scientifically—wavelengths, neural processing, physics, etc. When Mary finally leaves her room and sees color for the first time, does she learn something new?

This experiment translates that question into an empirical, interactive experience: Can you truly "know" colors through sound alone, or does seeing them teach you something fundamentally new?

## ✨ Features

### 1. **Color-to-Sound Mapping System**
- **Hue → Frequency**: Red (200Hz) to Purple (500Hz)
- **Saturation → Harmonic Richness**: More saturated colors have richer harmonics
- **Brightness → Volume/Amplitude**: Brighter colors are louder
- Powered by **Tone.js** for high-quality audio synthesis

### 2. **Multiple Audio Synthesis Modes**
Choose from three different sound generation approaches:
- **Pure Tones**: Simple sine waves (abstract, minimal)
- **Harmonic Rich**: Multiple harmonics (musical, complex)
- **FM Synthesis**: Frequency modulation (bell-like, distinctive)

### 3. **Training Mode**
- Interactive color swatches with playable sounds
- Progress tracking (requires 3+ plays per color)
- Optional **Blindfold Mode**: Hide visual colors during training
- Keyboard shortcuts for rapid learning

### 4. **Practice Mode**
- Test yourself with immediate feedback
- Track accuracy in real-time
- Requires 70%+ accuracy over 15 attempts to proceed
- Learn from mistakes

### 5. **Formal Test Mode**
- 20-question blind assessment
- Three difficulty levels:
  - **Easy**: 7 distinct hues
  - **Medium**: + brightness variations
  - **Hard**: + saturation variations
- No feedback until completion

### 6. **The Reveal Moment**
- Experience "Mary leaving the room"
- See actual colors for the first time
- Reflect on the phenomenological difference

### 7. **Philosophical Reflection**
Journal prompts exploring:
- What did colors "feel like" before seeing them?
- Did seeing them teach you something new?
- The nature of qualia and the knowledge argument

### 8. **Data Collection & Export**
- Complete accuracy metrics
- Learning curves
- Timestamped responses
- Export as JSON (for academic use)
- Human-readable text reports

## 🚀 Getting Started

### Requirements
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Working audio output (speakers or headphones)
- ~20-30 minutes for full experiment

### Installation

**Option 1: Direct Use**
Simply open `index.html` in your web browser. No build step required!

```bash
# Clone or download this repository
cd Mary_Room

# Open in browser
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

**Option 2: Local Server (Recommended)**
For best performance, serve via HTTP:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (if you have npx)
npx serve

# Then open http://localhost:8000
```

## 🎯 How to Use

### The Experiment Flow

1. **Introduction**
   - Learn about Mary's Room thought experiment
   - Understand the philosophical stakes

2. **Audio Mode Selection**
   - Choose your preferred synthesis method
   - Preview each option

3. **Training Mode**
   - Play each of the 7 colors at least 3 times
   - Memorize the sound-color associations
   - Optional: Enable Blindfold Mode for a purer experiment

4. **Practice Mode**
   - Test yourself with immediate feedback
   - Build confidence and accuracy
   - Must achieve 70%+ accuracy to proceed

5. **Pre-Test Reflection**
   - Describe what you think colors "are" based on sound alone
   - Important philosophical data point

6. **Formal Test**
   - 20 questions, no feedback
   - Demonstrates your functional knowledge

7. **The Reveal**
   - See colors for the first time
   - The "Mary leaves the room" moment

8. **Post-Test Reflection**
   - Did you learn something new?
   - Compare sonic vs. visual experiences
   - Reflect on qualia and phenomenal consciousness

9. **Results & Export**
   - View your performance
   - Export data for analysis

### Keyboard Shortcuts

**Training Mode:**
- `1-7`: Play colors 1-7
- `Space`: Replay last color

**Practice/Test Mode:**
- `Space` or `P`: Play current sound

## 📊 Data Export

The tool exports two types of data:

### JSON Export
Complete experimental data including:
```json
{
  "metadata": {
    "timestamp": "ISO-8601",
    "duration": "milliseconds",
    "audioMode": "sine|harmonic|fm",
    "difficulty": "easy|medium|hard"
  },
  "training": { "plays": {...}, "totalSoundPlays": 0 },
  "practice": { "accuracy": 0.0, "history": [...] },
  "test": { "accuracy": 0.0, "answers": [...] },
  "journals": { ... },
  "colors": [...]
}
```

### Text Report
Human-readable summary with:
- Performance statistics
- All journal responses
- Philosophical context
- Proper citation

## 🎨 The Color-Sound Mappings

| Color  | Frequency | Hue | RGB           |
|--------|-----------|-----|---------------|
| Red    | 200 Hz    | 0°  | rgb(255,0,0)  |
| Orange | 250 Hz    | 30° | rgb(255,165,0)|
| Yellow | 300 Hz    | 60° | rgb(255,255,0)|
| Green  | 350 Hz    | 120°| rgb(0,255,0)  |
| Cyan   | 400 Hz    | 180°| rgb(0,255,255)|
| Blue   | 450 Hz    | 240°| rgb(0,0,255)  |
| Purple | 500 Hz    | 270°| rgb(128,0,128)|

The mappings are:
- **Consistent**: Same color always produces same sound
- **Systematic**: Frequency increases linearly with hue
- **Learnable**: Users typically achieve 70-90% accuracy

## 🔬 Scientific & Educational Use

### For Researchers
- Empirical investigation of the knowledge argument
- Cross-modal perception studies
- Qualia research
- Philosophy of mind pedagogy

### For Educators
- Interactive philosophy of mind demonstrations
- Consciousness studies
- Epistemology (kinds of knowledge)
- Phenomenology

### For Students
- Hands-on engagement with abstract concepts
- Personal phenomenological data
- Critical thinking about consciousness

## 📚 Philosophical Background

### The Knowledge Argument

Frank Jackson's argument (simplified):

1. Mary knows all physical facts about color
2. Mary learns something new when she sees color
3. Therefore, there are non-physical facts (qualia)
4. Therefore, physicalism is false

### Responses & Debates

**Physicalist Responses:**
- **Ability Hypothesis** (Lewis, Nemirow): Mary gains abilities, not facts
- **Old Fact/New Guise**: She knew the fact, just experiences it differently
- **Phenomenal Concepts**: Different concepts, same fact

**Dualist Arguments:**
- The "explanatory gap" between physical and phenomenal
- The irreducibility of subjective experience
- Property dualism vs. substance dualism

### This Experiment's Contribution

By allowing functional mastery (accurate identification) without phenomenal experience, we can ask:
- Is functional knowledge sufficient?
- Does seeing colors add new information?
- Are qualia essential or epiphenomenal?

## 🎓 Citations

**Primary Source:**
```
Jackson, F. (1982). "Epiphenomenal Qualia."
Philosophical Quarterly, 32(127), 127-136.
```

**Related Reading:**
```
Jackson, F. (1986). "What Mary Didn't Know."
Journal of Philosophy, 83(5), 291-295.

Dennett, D. C. (1991). Consciousness Explained.
Boston: Little, Brown and Company.

Nagel, T. (1974). "What Is It Like to Be a Bat?"
Philosophical Review, 83(4), 435-450.

Chalmers, D. (1996). The Conscious Mind.
Oxford University Press.
```

## 🛠️ Technical Details

### Technologies Used
- **Pure HTML/CSS/JavaScript** (no build required)
- **Tone.js** v14.8 (audio synthesis)
- **CSS Grid & Flexbox** (responsive layout)
- **Web Audio API** (via Tone.js)
- **LocalStorage** (optional session persistence)

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

### Audio Synthesis
The tool uses three synthesis approaches:

1. **Sine Wave**: `new Tone.Synth({ oscillator: { type: 'sine' } })`
2. **Harmonic**: Fundamental + 2nd/3rd harmonics
3. **FM Synthesis**: Frequency modulation with modulationIndex: 10

### Accessibility
- Keyboard navigation throughout
- ARIA labels (where applicable)
- High contrast mode compatible
- Screen reader friendly (mostly)

## 🤝 Contributing

This is a philosophical/educational tool. Contributions welcome for:
- Additional audio synthesis modes
- Difficulty variations
- Accessibility improvements
- Localization/translation
- Scientific data analysis tools

## 📜 License

This project is released into the **public domain** for educational and research use.

Feel free to:
- Use in academic courses
- Modify for research
- Include in philosophy demonstrations
- Adapt for related experiments

**Attribution appreciated but not required.**

If publishing research using this tool, please cite:
```
Mary's Room: A Chromatic Qualia Experiment (2024)
Interactive philosophical thought experiment tool
https://github.com/[your-repo]
```

## 🙏 Acknowledgments

- **Frank Jackson** for the original thought experiment
- **Tone.js** developers for excellent audio tools
- The philosophy of mind community
- All participants who've contributed data and reflections

## 📧 Contact & Discussion

Questions, comments, or philosophical debates?

- Open an issue for technical problems
- Discussions welcome for philosophical interpretations
- Share your results and reflections!

---

## 💭 A Final Question

After completing this experiment, what do *you* think?

Did Mary learn something new when she saw red for the first time?

Or had she already captured everything essential through the sonic representations?

**There's no right answer—only your experience.**

---

**Enjoy exploring the nature of consciousness! 🧠🎨🔊**
