---
layout: default
title: Home
---

<style>
.home-container {
    min-height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    padding: 2rem;
}

.center-logo {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 1;
}

.center-logo img {
    max-width: 250px;
    width: 100%;
}

.corner-button {
    position: absolute;
    padding: 1.5rem 2rem;
    border-radius: 12px;
    text-decoration: none;
    color: white;
    font-weight: bold;
    font-size: 1.1rem;
    transition: transform 0.3s;
}

.corner-button:hover {
    transform: scale(1.05);
}

.btn-green {
    background: #4CAF50;
}

.btn-orange {
    background: #FF9800;
}

.top-left {
    top: 10%;
    left: 10%;
}

.top-right {
    top: 10%;
    right: 10%;
}

.bottom-left {
    bottom: 10%;
    left: 10%;
}

.bottom-right {
    bottom: 10%;
    right: 10%;
}

/* Mobile layout */
@media (max-width: 768px) {
    .home-container {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto auto;
        gap: 1rem;
        padding: 1rem;
        min-height: 80vh;
        align-items: center;
    }
    
    .center-logo {
        position: relative;
        top: auto;
        left: auto;
        transform: none;
        grid-column: 1 / 3;
        grid-row: 2;
        justify-self: center;
        z-index: 1;
    }
    
    .center-logo img {
        max-width: 150px;
    }
    
    .corner-button {
        position: relative;
        top: auto !important;
        left: auto !important;
        right: auto !important;
        bottom: auto !important;
        width: 100%;
        text-align: center;
        padding: 1rem;
        font-size: 0.9rem;
    }
    
    .top-left {
        grid-column: 1;
        grid-row: 1;
    }
    
    .top-right {
        grid-column: 2;
        grid-row: 1;
    }
    
    .bottom-left {
        grid-column: 1;
        grid-row: 3;
    }
    
    .bottom-right {
        grid-column: 2;
        grid-row: 3;
    }
}
</style>

<div class="home-container">
    <!-- Center logo -->
    <a href="/us/" class="center-logo">
        <img src="/assets/images/REDES%20Aless%205.png" alt="ReDes Logo">
    </a>
    
    <!-- Solarpunk - top left -->
    <a href="/solarpunk/" class="corner-button btn-green top-left">
        Solarpunk
    </a>
    
    <!-- Resources - top right -->
    <a href="/resources/" class="corner-button btn-orange top-right">
        Resources
    </a>
    
    <!-- Permaculture - bottom left -->
    <a href="/permaculture/" class="corner-button btn-green bottom-left">
        Permaculture
    </a>
    
    <!-- Sociocracy - bottom right -->
    <a href="/sociocracy/" class="corner-button btn-green bottom-right">
        Sociocracy
    </a>
</div>
