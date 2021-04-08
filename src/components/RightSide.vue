<template>
    <div class="right-side px-16 py-24">
        <Header />
        <SearchBar class="mt-16"/>
        <main class="mt-16">
            <div class="title font-bold" style="font-size: 40px">Discover new</div>
            <ul class="tabs mt-8 text-xl flex space-between" style="color: #686F75">
                <li class="tab active">Places</li> 
                <li class="tab">Experiences</li> 
                <li class="tab">Homes</li>    
            </ul>
            <div class="cards">
                <Card />
            </div>
        </main>
    </div>
</template>

<script>
import SearchBar from './SearchBar';
import Header from './Header';
import Card from './Card';

export default {
    name: 'RightSide',
    components: {
        SearchBar,
        Header,
        Card
    }
}
</script>

<style scoped>
    .right-side {
        max-width: 535px;
    }
    .tab {
        @apply mr-8;
    }
</style>