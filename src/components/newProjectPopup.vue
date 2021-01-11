<template>
  <v-dialog v-model="dialog" width="40%" >
        <v-card ref="form" class="pt-4">
          <v-card-text>
            <v-text-field
              ref="projectName"
              v-model="projectName"
              :rules="[() => !!name || 'This field is required']"
              label="Project Name"
              required
            ></v-text-field>
            <v-text-field
              ref="Version"
              v-model="Version"
              :rules="[() => !!name || 'This field is required']"
              label="Version"
              required
            ></v-text-field>
            <v-autocomplete
              ref="Teams"
              v-model="Teams"
              :rules="[() => !!Teams || 'This field is required']"
              :items="Teams"
              label="Teams"
              placeholder="Select..."
              required
            ></v-autocomplete>
            <v-text-field
              ref="gitUrl"
              v-model="gitUrl"
              :rules="[() => !!gitUrl || 'This field is required']"
              label="Git url"
              required
            ></v-text-field>
          </v-card-text>
          <v-card-actions>
            <v-btn text> Cancel </v-btn>
            <v-spacer></v-spacer>
            <v-slide-x-reverse-transition>
              <v-tooltip v-if="formHasErrors" left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn
                    icon
                    class="my-0"
                    v-bind="attrs"
                    @click="resetForm"
                    v-on="on"
                  >
                    <v-icon>mdi-refresh</v-icon>
                  </v-btn>
                </template>
                <span>Refresh form</span>
              </v-tooltip>
            </v-slide-x-reverse-transition>
            <v-btn color="primary" text @click="submit"> Submit </v-btn>
          </v-card-actions>
        </v-card>
  </v-dialog>
</template>

<script>
export default {
  data() {
    return {
      projectName: null,
      Teams: ["Devops", "Zenzura", "Alfa", "Omek", "Hi", "Drive", "Other"],
      gitUrl: null,
      dialog: false,
    };
  },
  methods: {
    showModal() {
      this.dialog = true;
    },
  },
};
</script>
