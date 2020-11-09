<template>
  <div class="container">
    <div>
      <client-only>
        <vue-html2pdf
          :show-layout="false"
          :enable-download="false"
          :preview-modal="true"
          :paginateElementsByHeight="1200"
          :manual-pagination="true"
          :html-to-pdf-options="htmlToPdfOptions"
  
          @progress="onProgress($event)"
          @hasStartedGeneration="hasStartedGeneration()"
          @hasGenerated="hasGenerated($event)"
          ref="html2Pdf"
        >
          <section slot="pdf-content">
            <section class="pdf-item">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Reiciendis iure aliquam cumque omnis, mollitia excepturi dolorum dicta deleniti deserunt dolore
              aut consequuntur impedit quod dolor cupiditate. Repudiandae ullam ipsum repellendus inventore, blanditiis 
              tempore facilis qui cupiditate ex adipisci magnam pariatur odio velit omnis error ad maiores dolorum aut 
              expedita nostrum atque! Nisi odio nesciunt dicta autem. Fuga corporis quaerat nam atque sunt quis illo. A
              libero veritatis aliquam modi eum quam commodi ipsum porro, aspernatur sed quibusdam hic molestias temporibus
              quasi voluptatibus cumque ratione! Possimus dolorem nobis beatae, rem repudiandae, officiis accusamus minus
              velit ut repellat doloremque, vitae aspernatur sed aliquam tenetur nemo! Cum minus, molestiae nihil earum et
              voluptatibus ducimus iure saepe rem! Atque repudiandae numquam a ab, mollitia tempora iste tenetur hic totam
              quod officia saepe harum quibusdam nam dolores voluptate unde et quos itaque, consequatur, suscipit magnam
              obcaecati ipsum tempore! Modi optio ullam provident reiciendis, dolore nesciunt est reprehenderit. Aliquid
              magni quo omnis mollitia minima, maiores odio itaque, repellendus nihil numquam debitis architecto ad 
              repudiandae illo, perferendis perspiciatis dolor adipisci velit! Dolore sint tempore blanditiis fugiat 
              incidunt optio voluptatum unde ad sunt rerum dignissimos praesentium vel consequatur suscipit corporis,
              sit obcaecati a architecto eveniet excepturi ea. Harum enim voluptate vitae placeat? Perferendis tenetur
              perspiciatis in beatae nam sunt, id, neque error corrupti quas pariatur non omnis, aut repellendus quod!
              Deleniti non enim error, ratione perferendis dolores rem libero voluptatum repudiandae, 
              itaque quis laudantium odit rerum dignissimos, est minus recusandae vero cumque voluptates 
              porro quaerat eligendi? Expedita doloremque cupiditate accusantium cum cumque fuga perspiciatis aperiam error ratione 
              eligendi facere, suscipit distinctio nisi dolores repellat perferendis, voluptas natus incidunt aliquid, id possimus vero.
              Voluptates iste error reprehenderit ut illum veritatis minima magni, accusantium dolorum mollitia cupiditate in. Quae aliquam
              corrupti ut ea voluptatem earum ex itaque debitis vitae est? Iste nostrum minus nam impedit earum aspernatur, nisi quaerat
              laborum velit veniam obcaecati consequuntur vel consectetur voluptas tempora sunt id distinctio ad deserunt necessitatibus,
              quo dicta suscipit! Amet nesciunt accusamus commodi dolore quas ducimus tempore eveniet modi minima tenetur eligendi deserunt
              iusto culpa soluta sit odit, qui officiis nemo illum dicta cumque quam natus? Praesentium obcaecati magni et saepe molestias
              libero aperiam esse nisi quam laborum. Eius veniam, molestiae reprehenderit atque aspernatur vitae et officiis possimus, numquam
              dicta eveniet quas laboriosam eos? Reprehenderit ipsam, repudiandae magnam natus eveniet architecto qui dicta. Quisquam dicta
              nemo harum sequi praesentium facilis aperiam porro? Provident dolorum explicabo asperiores praesentium rerum facere officiis,
              odio tempora, sequi laudantium id animi. Eum a hic esse quia voluptates eligendi beatae delectus nam! Fugit magni repellendus
              quod necessitatibus quibusdam, architecto expedita dolores excepturi est, doloribus vero aliquid numquam fuga aliquam minus
              dolore asperiores sunt? Recusandae beatae maiores inventore quia fuga placeat voluptatem ut unde aliquid vero dolores quasi
              cum, totam possimus, sapiente amet! Perferendis omnis error optio adipisci qui asperiores, aliquam magni iste nemo accusantium
              consequatur labore accusamus magnam et, a sequi. Et quidem magnam at! Reprehenderit, magni iusto et sequi maxime quo in odit est iste facere modi aspernatur
              unde inventore, nostrum quae numquam aperiam nobis quidem. Nesciunt laborum, dicta cum nam dignissimos maxime cupiditate, amet hic, suscipit voluptatem
              doloremque exercitationem. Sed ratione soluta distinctio maxime minus eius, veniam incidunt sint tempore voluptatibus odit facere obcaecati sapiente in numquam
              cupiditate tempora, vel deserunt nobis officia. Sequi harum deserunt dolorum reprehenderit maxime praesentium excepturi est, fuga soluta vel aliquam commodi?
              Officiis, quam earum sint deleniti labore numquam quaerat molestiae, adipisci qui inventore quidem libero eligendi tempora! Labore quos perspiciatis hic autem
              consectetur, placeat distinctio fuga, itaque, dolore laborum atque unde ut ex doloremque quam? Perferendis mollitia neque incidunt inventore quasi culpa fugiat,
              molestiae deserunt iure enim sit eaque placeat autem, omnis facilis excepturi tempore voluptas id minus iste dicta quam unde! Velit veniam dolorem fugit deleniti,
              optio vitae, quisquam amet, voluptatum architecto placeat non facere quibusdam sed! Impedit in exercitationem nostrum dicta architecto modi similique sint, ab
              labore quasi illo, ad a! Quasi nam ipsam quis quod blanditiis? Quae velit sequi pariatur cupiditate nisi facilis, possimus eius quam. Veniam non tempore saepe
              corporis nemo? Blanditiis placeat possimus voluptatum, dolorem earum officia doloremque sint sed voluptatibus, qui repellat! Expedita enim voluptatem sapiente
              sequi fugit ea! Laborum corporis debitis tenetur molestias alias distinctio eaque enim cum, quisquam ullam beatae, dolorum deserunt dignissimos nihil facilis
              aspernatur consequatur adipisci placeat ipsam similique esse possimus illum! Magni, voluptatem laborum! Saepe perspiciatis obcaecati pariatur quisquam eius
              praesentium animi minus ducimus cumque soluta quae suscipit nemo, in corporis? At iusto soluta consequatur sed ipsum culpa suscipit minus dignissimos doloribus
              inventore, ullam sunt laborum, odio quis, itaque rerum? Ducimus animi, voluptatem alias sit illo tenetur modi doloremque error porro ipsa quis voluptas in
              quibusdam minima dolores, a adipisci? Facere autem non repellendus maxime accusamus suscipit dolorem sapiente quo magni dolore rem corporis, asperiores
              voluptate nam debitis dolor placeat earum praesentium iste expedita fugiat quia in. Totam excepturi vitae nemo explicabo molestias eaque quia, ut facilis
              accusamus unde maiores illum corrupti eius nulla magni! Pariatur numquam, tempora eum culpa reprehenderit consequuntur quia aperiam nisi officia veniam.
              Sunt excepturi, animi commodi, quo incidunt aliquid sint aliquam earum quibusdam tempore quis nostrum voluptates nulla. Culpa enim facilis blanditiis
              sed atque qui repudiandae? Quas ut veniam et exercitationem, accusamus sint consequuntur magnam dolorum quam sed soluta tempora quod, dignissimos
              repellat repellendus, officia neque nam perspiciatis? Provident recusandae et praesentium suscipit illum quo nesciunt quis delectus eligendi iusto.
              Corrupti quasi aliquam voluptatum distinctio. Sunt aliquid illum sapiente rem, voluptas possimus quos iste nisi a ad, provident itaque ut temporibus
              dolores totam quaerat reiciendis consequatur quidem et molestiae ab error excepturi architecto sequi! Veniam, hic modi? Quia provident dolorem 
              suscipit maiores ipsa vitae eveniet fugit nesciunt iusto non alias dignissimos reprehenderit tempore esse nam doloribus cum inventore pariatur,
              cupiditate repellat labore omnis unde impedit culpa. Libero quos asperiores commodi dolore quidem quaerat alias accusamus. Recusandae excepturi 
              optio voluptas officia debitis iusto incidunt quibusdam dignissimos nesciunt. Ut nesciunt explicabo perferendis autem voluptates cumque omnis
              quis eum sint quisquam. Nesciunt ipsa ab sequi dolor assumenda.
            </section>
          </section>
        </vue-html2pdf>
      </client-only>

    <button style="display: block; margin: 9 auto; padding: 15px; border: 1px solid #555; border-radius: 5px;" @click="generatePdf()">
      Generate PDF
    </button>
    </div>
  </div>
</template>

<script>
import PdfContent from '@/components/PdfContent'
export default {
  components: {
    PdfContent
  },

  data() {
    return {
      htmlToPdfOptions: {
        margin: [0, 0, 0.3, 0],
    
        filename: `hehehe.pdf`,
    
        image: {
            type: 'jpeg', 
            quality: 0.98
        },
    
        html2canvas: {
            scale: 1,
            useCORS: true
        },
    
        jsPDF: {
            unit: 'in',
            format: 'a4',
            orientation: 'portrait'
        }
      }
    }
  },

  methods: {
    generatePdf () {
      this.$refs.html2Pdf.generatePdf()
    },

    onProgress (x) {
      console.log(x)
    },

    hasGenerated (x) {
      console.log(x)
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
