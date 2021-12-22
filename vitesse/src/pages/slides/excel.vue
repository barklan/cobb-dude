<template>
    <div class="row-container">
        <iframe
            class="second-row"
            src="https://nervous-tereshkova-2a5415.netlify.app/"
            title="description"
        ></iframe>
    </div>
</template>

<style>

body, html {
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none;  /* Firefox */
}

 /* Hide scrollbar for Chrome, Safari and Opera */
.row-container::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.second-row::-webkit-scrollbar {
  display: none;
}
.row-container {
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none;  /* Firefox */
    display: flex;
    width: 100%;
    min-height: 87vh;
    flex-direction: column;
    overflow: hidden;
}
.second-row {
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none;  /* Firefox */
    display: block;
    flex-grow: 1;
    min-height: 100%;
    border: none;
    margin: 0;
    padding: 0;
}
</style>
