<template>
  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card bg-secondary text-white">
      <q-card-section>
        <div class="text-h6">Sketchbook #1</div>
        <div class="text-subtitle2">by MoC</div>
      </q-card-section>

      <q-card-section>
        {{ props.lorem }}
      </q-card-section>

      <q-separator dark />

      <q-card-actions>
        <q-btn flat>Edit</q-btn>
        <q-btn flat>Delete</q-btn>
      </q-card-actions>
    </q-card>

    <q-card class="my-card">
      <q-card-section>
        <div class="text-h6">Sketchbook #</div>
        <div class="text-subtitle2">by MoC</div>
      </q-card-section>

      <q-separator />

      <q-card-actions vertical>
        <q-btn flat>Edit</q-btn>
        <q-btn flat>Delete</q-btn>
      </q-card-actions>
    </q-card>

    <q-card class="my-card bg-purple text-white">
      <q-card-section>
        <div class="text-h6">Sketchbook #</div>
        <div class="text-subtitle2">by MoC</div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat>Edit</q-btn>
        <q-btn flat>Delete</q-btn>
      </q-card-actions>
    </q-card>

    <q-card flat bordered class="my-card" :class="$q.dark.isActive ? 'bg-grey-9' : 'bg-grey-2'">
      <q-card-section>
        <div class="row items-center no-wrap">
          <div class="col">
            <div class="text-h6">Our Planet</div>
            <div class="text-subtitle2">by MoC</div>
          </div>

          <div class="col-auto">
            <q-btn color="grey-7" round flat icon="more_vert">
              <q-menu cover auto-close>
                <q-list>
                  <q-item clickable>
                    <q-item-section>Remove Card</q-item-section>
                  </q-item>
                  <q-item clickable>
                    <q-item-section>Send Feedback</q-item-section>
                  </q-item>
                  <q-item clickable>
                    <q-item-section>Share</q-item-section>
                  </q-item>
                </q-list>
              </q-menu>
            </q-btn>
          </div>
        </div>
      </q-card-section>

      <q-card-section>
        {{ props.lorem }}
      </q-card-section>

      <q-separator />

      <q-card-actions>
        <q-btn flat>Edit</q-btn>
        <q-btn flat>Delete</q-btn>
      </q-card-actions>
    </q-card>
  </div>
</template>

<script setup>
defineOptions({
  name: 'CardsActions'
})

const props = defineProps({
  lorem: {
    type: String,
    default: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  }
})
</script>


<!-- <script>
export default {
  setup () {
    defineOptions({
      name: 'CardsActions'
    })
    return {
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
    }
  }
}
</script> -->
