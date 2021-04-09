<template>
    <div class="right-side px-16 py-24">
        <Header />
        <SearchBar class="mt-16"/>
        <main class="mt-16">
            <div class="title font-bold" style="font-size: 40px">Discover new</div>
            <TabNav class="mt-8" :tabs="['Places', 'Experiences', 'Home']" :selected="selected" @selected="setSelected" >
                <Tab :isSelected="selected === 'Places'" >
                    <CardsCarousel>
                        <Card></Card>
                        <Card></Card>
                        <Card></Card>
                    </CardsCarousel>
                </Tab>
                <Tab :isSelected="selected === 'Experiences'" >
                    <h1>More test text</h1>
                </Tab>
                <Tab :isSelected="selected === 'Home'" >
                    <ul>
                        <li>List test 1</li>
                        <li>List test 2</li>
                        <li>List test 3</li>
                    </ul>
                </Tab>
            </TabNav>
        </main>
    </div>
</template>

<script>
import SearchBar from './SearchBar';
import Header from './Header';
import TabNav from './TabNav';
import Tab from './Tab.vue';
import CardsCarousel from './CardsCarousel';
import Card from './Card';

export default {
    name: 'RightSide',
    components: {
        SearchBar,
        Header,
        TabNav,
        Tab,
        CardsCarousel,
        Card,
    },
    data() {
        return {
            selected: 'Places'
        }
    },
    methods: {
        setSelected(tab) {
            this.selected = tab;
        }
    }
}
</script>

<style scoped>
    .right-side {
        max-width: 535px;
    }
</style>