# 🃏 RenzUwU’s ComfyUI Workflows

ComfyUI Workflow Drop: FREE I2I Wan 2.2 ClownShark Realistic Waifu Generator v2 by RenzUwU
So I got bored and started looking at other people’s posts… and yeah I basically just copied homework and taped some glitter on it 🤡
This one is the image-to-image version of my earlier text workflow:
1. Load Image → shove through Florence 2 → spit out text → Prompt Replace node.
   ➤ Example: your ref has “blonde hair,” just type it in “Find” and swap to whatever you want in “Replace.”
   ➤ Downside: body types need to be roughly the same. Otherwise… clown results.
2. Prompt Combine → throw in trigger words / sauce → text encoder for positive.
   ➤ Negatives still same as before (don’t overthink it, it just works™).
3. Image Resize → 0.92MP sweet spot. Go over that and the model starts cooking cursed meals. (I left notes in the graph.)
4. First ClownSharkSampler (2 steps, bong_tangent).
   ➤ Smashes the image, keeps ~50% noise, and for some reason looks cleaner. Todd Howard already said it best: *it just works.*
5. Latent Scale (Pixel Space) → upscale 1.5x.
6. Second KSampler (4 steps) to denoise fully.
   ➤ You could skip sampler 1, but colors/details go weird so I keep it. (Probably my lightx2v is too high but eh 🤡).
Everything else matches the T2I workflow, but I swear this one feels cleaner. Maybe placebo, maybe science.
---

⚠️ Disclaimer:
I don’t code. I have no idea what I’m doing. I just mash nodes until something decent comes out. It just works™ eventually.

---

### Want more?

👉 Full write-ups, notes, and lore are here: [https://ovi1.site/](https://ovi1.site/)

👉 If you like what I’m doing (or just want to fund my next pack of instant noodles), you can throw coins here: [https://ko-fi.com/renzuwu](https://ko-fi.com/renzuwu)

---

Use at your own risk. If it breaks, that’s probably your fault… or mine… or Wan’s.
