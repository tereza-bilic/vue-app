url aplikacije: https://task-app-ps8b.onrender.com/

1. interpolation/one-way binding:
	Da, src/views/Home.vue :11
2. two-way binding:
	Da, src/compontents/TaskForm.vue :3 Koristi se v-model za newTask koji je dvosmjerno povezan s inputom za unos taska, a u :18-:20 je funkcija koja definira data property
3. methods:
	Da, src/views/Home.vue :41, funkcije addTask i markAsCompleted
4. computed properties:
	Da, src/views/Home.vue :36 completedTasksCount
5. barem jedan scoped style:
	Da, src/components/TaskList.vue :25-:40
6. koristiti barem jedan lifecycle hook:
	Da, u src/views/Home :53 updated() - za spremanje taskova u local storage i :56 mounted() za dohvaćanje iz localstoragea
7. routing (više stranica)
  - aplikacija mora biti bookmarkable, tako da rade linkovi (ne samo na root, već i moj-web.com/stranica1, moj-web.com/stranica2):
		Da, postoje 3 stranice index tj. '/', 'page1' i 'page2'
  - dinamičko usmjeravanje s 404 stranicom ("catch all"):
		Da, postoji catch all
8. (barem) dvije komponente
 - komponenta bez stanja, koristiti properties:
		Da, src/compontents/TaskList prima prop tasks
 - komponenta sa stanjem
 		Da, src/components/TaskForm ima state
9. barem jedna komponenta mora emitirati barem jedan event:
	Da, src/components/TaskForm emitira dodavanje taska :17
10. store (Pinia):
	Ne
11. asinkroni dohvat podataka s backenda, možete:
	Ne
- koristiti Firebase ili Back4App, Mocky, itd.
- vlastiti storage, ili
- možete mock napraviti, držati podatke u memoriji, ali mora biti asinkroni poziv/upis
ostvariti asinkrono (lazy, po potrebi) učitavanje nekog dijela aplikacije (stranice ili komponente)
