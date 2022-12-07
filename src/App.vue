<template>
    <FirstComponent />
    <LifeCycle />
</template>

<script>

import FirstComponent from "./components/FirstComponent";
import LifeCycle from "./components/LifeCycle";

export default{
    name: 'App',
    components: {
        FirstComponent,
        LifeCycle
    }
}
</script>
