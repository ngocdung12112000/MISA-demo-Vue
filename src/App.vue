<template>
    <div id="app">
        <TheNavbar />
        <TheHeader />
        <TheContent />
        <TheDialog/>
    </div>
</template>

<script>
import TheNavbar from './components/layout/TheNavbar.vue'
import TheHeader from './components/layout/TheHeader.vue'
import TheContent from './components/layout/TheContent.vue'
import TheDialog from './components/layout/TheDialog.vue'

export default {
    name: 'App',
    components: {
        TheNavbar,
        TheHeader,
        TheContent,
        TheDialog
    }
}
</script>

<style>
@import './style/base/button.css';
@import './style/base/table.css';
@import './style/base/input.css';
@import './style/base/dialog.css';

body {
    margin: 0;
}

.bg-primary {
    background-color: #01B075;
}

body{
    font-family: GoogleSans-Regular;
    font-size: 13px;
}

@font-face {
    font-family: 'GoogleSans-Regular';
    src: url('assets/font/GoogleSans-Regular.otf') format('opentype');
}

@font-face {
    font-family: 'GoogleSans-Bold';
    src: url('assets/font/GoogleSans-Bold.otf') format('opentype');
}

@font-face {
    font-family: 'GoogleSans-Italic';
    src: url('assets/font/GoogleSans-Italic.otf') format('opentype');
}

@font-face {
    font-family: 'GoogleSans-BoldItalic';
    src: url('assets/font/GoogleSans-BoldItalic.otf') format('opentype');
}

.bg-row-selected {
    background-color: #f0f0f0;
}
</style>
