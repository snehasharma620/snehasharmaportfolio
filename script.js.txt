window.addEventListener("scroll",()=>{
  document.querySelectorAll(".glass").forEach(box=>{
    let pos = box.getBoundingClientRect().top;
    if(pos < window.innerHeight-100){
      box.style.opacity = "1";
      box.style.transform = "translateY(0)";
    }
  });
});
