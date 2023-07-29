<template>
  <v-container style="display: flex; flex-direction: column; min-height: 100%">
    <v-row column wrap class="bg-white mt-3 pa-4" style="border-radius: 4px">
      <div class="enrollments-title stats-counter">
        Informações da matrícula
      </div>
      <div class="enrollments-subtitle stats-subtitle mb-2">
        Saiba mais sobre a concorrência nas disciplinas, turmas e cursos
        presentes na UFABC.
      </div>
    </v-row>
  </v-container>
</template>

<style>
.card-group-stats .card-stats:first-child,
.card-group-stats .card-stats:not(:first-child):not(:last-child) {
  border-right: 1px solid rgba(0, 0, 0, 0.03);
}

@media (min-width: 576px) {
  .card-group-stats > .card-stats:first-child {
    border-top-right-radius: 0;
    border-bottom-right-radius: 0;
  }
}
@media (min-width: 768px) {
  .card-group-stats .card-stats:first-child,
  .card-group-stats .card-stats:not(:first-child):not(:last-child) {
    border-right: 1px solid rgba(0, 0, 0, 0.03);
  }
}
@media (min-width: 576px) {
  .card-group-stats
    > .card-stats:not(:first-child):not(:last-child):not(:only-child),
  .card-group-stats
    > .card-stats:not(:first-child):not(:last-child):not(:only-child)
    .card-footer,
  .card-group
    > .card:not(:first-child):not(:last-child):not(:only-child)
    .card-header,
  .card-group
    > .card:not(:first-child):not(:last-child):not(:only-child)
    .card-img-bottom,
  .card-group
    > .card:not(:first-child):not(:last-child):not(:only-child)
    .card-img-top {
    border-radius: 0;
  }
}

.card-stats {
  position: relative;
  display: flex;
  flex-direction: column;
  min-width: 0;
  word-wrap: break-word;
  background-color: #fff;
  background-clip: border-box;
  border: 1px solid rgba(0, 0, 0, 0.125);
  border-radius: 0.25rem;
  border-radius: 4px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
  border: none;
  padding: 1.25rem;
}

.stats-counter {
  color: #455a64;
  font-size: 22px;
  font-weight: bold;
}
.stats-subtitle {
  font-weight: 300;
  color: #99abb4;
}

.enrollments-title {
  font-size: 26px;
}
.enrollments-subtitle {
  align-items: center;
  flex: none !important;
}

.load-more {
  border-top-left-radius: 0px;
  border-top-right-radius: 0px;
  border-top: none;
}
</style>
