<script>
    import Logo from "./Logo.svelte";
    import Link from "./Link.svelte";
</script>

<header>
        <div class="buttonsLeft">
            <Logo/>
            <nav class="navButtons">
                <Link text="Inicio"/>
                <Link text="Películas"/>
                <Link text="Series"/>
                <Link text="Colecciones"/>
                <Link text="Festivales"/>
                <Link text="Más"/>
                <svg xmlns="http://www.w3.org/2000/svg" width="14" height="10" viewBox="0 0 14 10" fill="none">
                    <path d="M13 1L7 9L1 0.999999" stroke="white" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
            </nav>
        </div>
        <div class="buttonsRight">
            <button class="buttonSubscribe">
                    SUSCRÍBETE
            </button>
                <button class="buttonlogIn">
                    INICIAR SESIÓN 
                </button>
                <svg class="searchIcon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
                    <path d="M23.6322 21.591L18.1915 16.1503C19.5014 14.4065 20.2085 12.284 20.2061 10.103C20.2061 4.53226 15.6738 0 10.103 0C4.53226 0 0 4.53226 0 10.103C0 15.6738 4.53226 20.2061 10.103 20.2061C12.284 20.2085 14.4065 19.5014 16.1503 18.1915L21.591 23.6322C21.8664 23.8783 22.2256 24.0098 22.5948 23.9994C22.9641 23.9891 23.3154 23.8378 23.5766 23.5766C23.8378 23.3154 23.9891 22.9641 23.9994 22.5948C24.0098 22.2256 23.8783 21.8664 23.6322 21.591ZM2.88658 10.103C2.88658 8.67576 3.30982 7.28053 4.10278 6.09379C4.89573 4.90705 6.02279 3.9821 7.34142 3.4359C8.66006 2.88971 10.111 2.7468 11.5109 3.02524C12.9108 3.30369 14.1966 3.99099 15.2058 5.00023C16.2151 6.00947 16.9024 7.29532 17.1808 8.69518C17.4593 10.095 17.3164 11.546 16.7702 12.8647C16.224 14.1833 15.299 15.3103 14.1123 16.1033C12.9255 16.8963 11.5303 17.3195 10.103 17.3195C8.18982 17.3172 6.35562 16.5562 5.00277 15.2033C3.64992 13.8505 2.88888 12.0163 2.88658 10.103Z" />
                </svg>
        </div>
</header>

<style>

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 16px 64px;
    }   

    .buttonsLeft {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        gap: 24px;
    }

    .navButtons {
        font-weight: 550;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .buttonsRight {
        gap: 16px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    .buttonSubscribe {
        font-weight: 800;
        border: none;
        border-radius: 4px;
        display: flex;
        height: 32px;
        padding: 0px 12px;
        justify-content: center;
        align-items: center;
        background: #02FFA1;
        cursor: pointer;
    }

    .buttonSubscribe:hover {
        background: #5EFFC3;
    }

    .buttonlogIn {
        font-weight: 800;
        color: #ffffff;
        display: flex;
        height: 32px;
        padding: 0px 12px;
        justify-content: center;
        align-items: center;
        border-radius: 4px;
        border: 2px solid #FFF;
        background: rgba(0, 0, 0, 0.00);
        cursor: pointer;
    }

    .buttonlogIn:active{
        background-color: #6F6F81;
    }

    .buttonlogIn:hover {
        border-color: #6F6F81;
    }

    .searchIcon {
        padding: 1px 0px 1px 6px;
        cursor: pointer;
        fill:white;
    }

    .searchIcon:hover {
        fill:#02FFA1;
    }
</style>