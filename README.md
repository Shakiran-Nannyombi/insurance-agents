# Insurance Risk Agents

Four agents: intake, extraction, risk, summary.

## Structure
- prompts/: system instructions and prompt per agent
- samples/: test inputs
- n8n/: exported flow
- app/: deployed web app
- docs/: notes and screenshots

## Build it in Agent Studio
1. Go to **Navigation menu, Agent Platform, Studio. Select New, then Chat.
2. Name the prompt (for example "Agent 1 Intake"). Paste the system instructions into the **System instructions** box. Paste the agent's Prompt into the main **Prompt** box, replacing the bracketed part with the sample note or the previous agent's output.
3. Set **Region** to Global. Set **Thinking level** to Low for extraction, High for the risk agent.
4. Submit, review, then Save.
5. Use **Compare** to test a changed instruction or a different model side by side.
6. Deploy, Cloud Run, Deploy as app. Open the app and test it with a new note.

> Menu and model names can change between console updates. Follow what you see on screen.

## For AntigravityIDE
Read the files in prompts/. Add a fifth agent that checks the Summary output against the original client note and flags any claim not supported by the note. Write its prompt in prompts/05-verifier.md in the same style as the others, then show me the diff.

## Try next
Add Grounding: Your data with a short underwrit ing guide.
Turn on structured outputs so every agent returns JSON.
Swap in your own industry: logistics, agriculture, health clinics.