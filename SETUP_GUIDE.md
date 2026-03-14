# Schrödinger Classes — Website Setup Guide

## 📁 Files Included
- `index.html` — Homepage
- `notes.html` — Chapter-wise notes
- `videos.html` — YouTube video lectures
- `quiz.html` — Interactive MCQ quizzes
- `test.html` — Full-length mock tests (JEE/NEET pattern)
- `simulation.html` — Physics simulations (Pendulum, Wave, Projectile)
- `login.html` — Student login/register (Firebase Auth)

---

## 🚀 Step 1: Put Website on GitHub Pages (FREE)

1. Go to https://github.com and **sign up / sign in**
2. Click **New Repository**
   - Name it: `schrodinger-classes` (or any name)
   - Set to **Public**
   - Click **Create Repository**
3. Click **uploading an existing file**
4. **Drag and drop all HTML files** into the browser
5. Click **Commit changes**
6. Go to **Settings → Pages**
7. Under "Branch", select **main** → Click **Save**
8. Your website is live at:
   `https://YOUR_GITHUB_USERNAME.github.io/schrodinger-classes/`

---

## 🔐 Step 2: Set Up Firebase (Student Login)

1. Go to https://console.firebase.google.com
2. Click **Add Project** → Name it "schrodinger-classes" → Continue
3. Go to **Authentication → Sign-in method**
4. Enable **Email/Password** ✅
5. Enable **Google** ✅
6. Go to **Project Settings** (gear icon)
7. Scroll down → Click **Add App** → Choose **Web** (</>)
8. Register app → Copy the `firebaseConfig` object
9. Open `login.html` in a text editor
10. Find this section:
    ```javascript
    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      ...
    };
    ```
11. Replace with your actual config from Firebase
12. Re-upload `login.html` to GitHub

---

## 🎬 Step 3: Add Your YouTube Videos

1. Open `videos.html`
2. Find cards like:
   ```html
   onclick="openVideo('VIDEO_ID_HERE', 'Title', 'Subject')"
   ```
3. Replace `VIDEO_ID_HERE` with your YouTube video ID
   - e.g. if URL is: `https://youtu.be/dQw4w9WgXcQ`
   - Video ID is: `dQw4w9WgXcQ`
4. Update the channel subscribe link:
   ```html
   href="https://youtube.com/@YOUR_CHANNEL_HANDLE"
   ```

---

## 📄 Step 4: Add Your PDF Notes

1. Create a `notes/` folder in your GitHub repo
2. Upload your PDF files there
3. Open `notes.html`
4. Find download buttons like:
   ```html
   <a class="note-dl" href="#" onclick="notifyUpload(event)">
   ```
5. Replace `href="#"` with:
   ```html
   href="notes/your-chapter-file.pdf" download
   ```
   Remove the `onclick` attribute too.

---

## ✏️ Step 5: Customize Your Info

In `index.html`, update:
- Stats (number of students, videos etc.)
- Teacher intro text

In `videos.html`:
- Replace "S" avatar with your photo if desired
- Update subscriber count

---

## ➕ Adding More Quiz Questions

Open `quiz.html`, find `const QUIZZES = [...]` and add:
```javascript
{
  id: 'gravitation', title: "Gravitation", course: "11",
  desc: "Kepler's laws, satellites, escape velocity", count: 5,
  questions: [
    {
      q: "Your question here?",
      options: ["Option A", "Option B", "Option C", "Option D"],
      ans: 0,  // 0 = A, 1 = B, 2 = C, 3 = D
      explanation: "Explanation here."
    },
    // ... more questions
  ]
}
```

---

## 📞 Need Help?
If you face any issues, contact support or ask in the GitHub Issues section of your repo.

**Your website URL will be:**
`https://YOUR_USERNAME.github.io/schrodinger-classes/`
