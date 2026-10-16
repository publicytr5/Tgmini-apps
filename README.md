# Viral Video Mini App — Flat GitHub Upload

এই প্যাকেজটি ফোনে extract ও GitHub-এ upload সহজ করার জন্য flat রাখা হয়েছে। `index.html`, JavaScript এবং CSS—তিনটি deploy ফাইল একই directory-তে থাকবে।

## GitHub-এ দিন
1. ZIP extract করুন।
2. GitHub repository খুলে **Add file → Upload files** চাপুন।
3. এই ZIP থেকে পাওয়া `index.html`, `index-CsNlnSIc.js`, `index-By6Vn5D-.css`—তিনটি ফাইল repository-র root-এ upload করে commit করুন। README.md চাইলে এটিও দিতে পারেন। ZIP-টি নিজে upload করবেন না।
4. যদি আগের upload-এ `assets/` folder, JS/CSS-এর duplicate, বা আগের `index.html` থাকে, পুরোনোগুলো মুছে নতুন flat ফাইলগুলো root-এ রাখুন।

## Vercel
GitHub commit হলে Vercel redeploy করবে। Framework **Other**, Build Command ফাঁকা, Output Directory `.` রাখুন। Deploy শেষে homepage এবং `/index-CsNlnSIc.js`, `/index-By6Vn5D-.css` path-গুলো 404 না হওয়া যাচাই করুন।
