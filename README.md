document.addEventListener("DOMContentLoaded", () => {
  const bays = document.querySelectorAll(".bay");

  bays.forEach(bay => {
    bay.addEventListener("click", () => {
      const status = bay.dataset.status;
      alert(`BAY ${bay.textContent} is ${status.toUpperCase()}`);
    });
  });

  document.getElementById("searchButton").addEventListener("click", () => {
    const name = document.getElementById("contractorName").value;
    const bay = document.getElementById("bayNumber").value;
    const result = document.getElementById("searchResult");

    // Dummy result (replace with real logic)
    result.textContent = `Searching for BAY ${bay}, Contractor: ${name}`;
  });
});
