<script>
	import Button from "$lib/components/ui/button/button.svelte";
    import { Input } from "$lib/components/ui/input";
    import * as Card from "$lib/components/ui/card";


</script>

<main class="grid grid-cols-1 gap-8 p-8 pt-16 md:grid-cols-4">

    <div class="flex flex-col gap-16">
    <div class="relative grid items-center grid-cols-2 gap-6 p-2 border border-dashed rounded-xl">
       
       <div class="absolute top-0 p-1 text-sm font-bold -translate-y-full">
        <h1 class="">Buttons</h1>
       
    </div> 
        <div><Button>Default</Button></div>
        <p>Default button</p>
        <div><Button variant="secondary">Secondary</Button></div>
        <p>Secondary button</p>
        <div><Button variant="ghost">Ghost</Button></div>
        <p>Ghost button</p>
        <div><Button variant="outline">Outline</Button></div>
        <p>Outline button</p>
        <div class="flex flex-row gap-2">
            <Button icon="heroicons:home" size="icon"></Button>
            <Button variant="outline" icon="heroicons:home" size="icon"></Button>
            <Button variant="ghost" icon="heroicons:home" size="icon"></Button>
        </div>
        <p>Icon button</p>

        
    </div>

    <div class="relative grid items-center grid-cols-2 gap-6 p-2 border border-dashed rounded-xl">
        <div class="absolute top-0 p-1 text-sm font-bold -translate-y-full">
         <h1 class="">Button Sizes</h1>
     </div> 
     <div><Button size="sm">Small</Button></div>
         <p>Small size</p>
         <div><Button>Default</Button></div>
         <p>Default size</p>
         
         <div><Button size="lg">Large</Button></div>
         <p>Large size</p>
     </div>

    

    
</div>

<div>
    <div class="relative grid items-center grid-cols-3 gap-1 p-2 text-white border border-dashed rounded-xl">
       
        <div class="absolute top-0 p-1 text-sm font-bold -translate-y-full">
            <h1 class="text-black">Button Sizes</h1>
        </div> 
         
        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-primary">
            <h1 class="color">primary</h1>
            <!-- <p></p> CHAT GPT, ADD HERE CSS COLOR OF ITEM ABOVE -->
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-secondary">
            <h1 class="color">secondary</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-muted">
            <h1 class="color">muted</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-popover">
            <h1 class="color">popover</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-card">
            <h1 class="color">card</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-border">
            <h1 class="color">border</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-accent">
            <h1 class="color">accent</h1>
        </div>
       
        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-destructive">
            <h1 class="color">destructive</h1>
        </div>

        <div class="flex items-center justify-center text-xs border aspect-square rounded-xl bg-ring">
            <h1 class="color">ring</h1>
        </div>

     </div>
</div>
     
<div>
    <div class="relative grid items-center grid-cols-1 gap-6 p-2 border border-dashed rounded-xl">
       
        <div class="absolute top-0 p-1 text-sm font-bold -translate-y-full">
         <h1 class="">Typography</h1>
        </div> 
         
         <h1>Heading 1</h1>

         <h2>Heading 2</h2>

         <h3>Heading 3</h3>

         <p>Base</p>
     </div>
</div>

<div>
    <div class="relative grid items-center grid-cols-2 gap-6 p-2 border border-dashed rounded-xl">
       
        <div class="absolute top-0 p-1 text-sm font-bold -translate-y-full">
         <h1 class="">Components</h1>
        </div> 
        
        <Input placeholder="Input" />
        <p>Input</p>

        <Card.Root>
            <Card.Header>
              <Card.Title>Card Title</Card.Title>
              <Card.Description>Card Description</Card.Description>
            </Card.Header>
            <Card.Content>
              <p>Card Content</p>
            </Card.Content>
            <Card.Footer>
              <p>Card Footer</p>
            </Card.Footer>
          </Card.Root>
          <p>Card</p>

          

        
     </div>
</div>
     
</main>

<style>
    p {
        font-size: 14px;
    }

    .color {
        mix-blend-mode: difference;
    }
</style>