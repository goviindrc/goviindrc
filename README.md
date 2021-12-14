- 👋 Hi, I’m @goviindrc
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
goviindrc/goviindrc is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
code for wall hack                   Main.children
[7].s38.b34.tBJ.radius=-0
code for fly hack code : var mc7,e

    tBJ,
    up = true;

function defineMc7() {
    mc7 = Main.children[7];

    if(mc7.s38 === null) setTimeout(defineMc7, 50);
    else tBJ = mc7.s38.b33.tBJ;
}
defineMc7();

function fly(e) {
    var state = (e.type == "keyw") ?true: false;

    if(e.code == "Key w") up = state;

    if(up) {
        tBJ.gravMass = -3;

        mc7.s38.I32 = "jump__in";
    }
    if(!up) {
        tBJ.gravMass =2;
         mc7.s38.I32 = "idle";
    }
}
window.addEventListener("keydown", fly);

window.addEventListener("keyup", fly);
