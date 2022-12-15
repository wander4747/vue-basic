<template>
    <Header />
    <FirstComponent />
    <LifeCycle />
    <People />
</template>

<script>

import FirstComponent from "./components/FirstComponent";
import LifeCycle from "./components/LifeCycle";
import People from "./components/People";
import Header from "./components/Header";

export default{
    name: 'App',
    components: {
        FirstComponent,
        LifeCycle,
        People,
      Header
    }
}
</script>
