<template>
    <FirstComponent />
    <LifeCycle />
    <People />
</template>

<script>

import FirstComponent from "./components/FirstComponent";
import LifeCycle from "./components/LifeCycle";
import People from "./components/People";

export default{
    name: 'App',
    components: {
        FirstComponent,
        LifeCycle,
        People
    }
}
</script>
