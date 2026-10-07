# Portfolio
This is my Portfolio

## Hugging Face Profile Panel (integrated)

The **Hugging Face** button in the top navigation opens an in-page Hugging Face
profile panel — no page navigation. It fetches your public Hugging Face profile
(user `Rumiii`) live from the Hugging Face API and shows:

- Your avatar, name (Rumi Iqbal Sufi), title (AI Engineer) and member-since date.
- Live stats: Models, Datasets, total all-time Downloads, total all-time Likes,
  and Followers.
- A searchable, sortable grid of every public model and dataset.
- Each card is clickable and opens the repository on huggingface.co.
- A **Details** button opens an opaque, fully-readable modal with the full
  repository overview, tags, base model, datasets used, etc.

### How it works
- `Index.html` contains everything (HTML + scoped CSS + vanilla JS). No build
  step, no backend — the Hugging Face public API supports browser CORS.
- `hf-wallpaper.png` is the AI-generated themed background for the panel.
- The panel's styles are scoped under `#hf-overlay` (`.hf-` prefix) so they
  never clash with the rest of the portfolio.

### Deploy
This is a static site — deploy the folder as-is to Netlify (or any static host).
