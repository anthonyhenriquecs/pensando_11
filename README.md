# pensando_11

body {
    height: 100vh;
    margin: 0;
    display: grid;
    place-content: center;
    background-color: #766b6b;
}

.loader {
    position: relative;
    height: 25px;
    width: 255px;
    font-family: Helvetica, system-ui;
}

.dot {
    position: absolute;
    height: 25px;
    width: 25px;
    background-color: var(--c);
    animation: loader 3s ease-in-out var(--d) infinite;
    border-radius: 100%;
    border: 2px solid white;
}

.text:after {
    position: absolute;
    content: "Loading";
    width: 4rem;
    font-weight: bold;
    top: 150%;
    left: 0;
    right: 0;
    margin: auto;
    animation: loanding-text 3s infinite;
}

@keyframes loader {
    15%{
        transform: translateX(0);
    }
    45% {
        transform: translateX(230px);
    }
    65% {
        transform: translateX(230px);
    }
    95% {
        transform: translateX(0);
    } 
}

@keyframes loandig-text {
    0% {
        content: "Loading";
    }

    25% {
        content: "Loading.";
    }

    50% {
        content: "Loading..";
    }

    75% {
        content: "Loading...";
    }
    
}
