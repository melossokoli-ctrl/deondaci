# Twitch Guide Bot (SQ/EN)

Chatbot qe pergjigjet VETEM per Twitch, me foto (ilustrime) dhe video (embed live i Twitch + linke video).

## Deploy ne Vercel
1. Ngarko keta skedare ne nje repo GitHub (index.html, api/chat.js, vercel.json).
2. Vercel -> New Project -> importo repon.
3. Settings -> Environment Variables -> `ANTHROPIC_API_KEY` = celesi yt. (Opsionale: `ANTHROPIC_MODEL`)
4. Redeploy. Pa API key boti punon me pergjigjet lokale (13 tema).

## Personalizim
- Kanali live: ndrysho `channel=twitch` te `TWITCH_EMBED` ne index.html.
- Tema te reja: shto nje objekt ne `KB` (keywords, sq, en, svg, video, link) dhe nje ilustrim ne `SVGS`.
- Video te tua: te `video:` vendos `yt:<kerkim>` (hap YouTube) ose nderro `fig` me nje `<iframe>` YouTube embed.
