<script setup>
</script>

<template>
  <div class="app">
    <header>
      <a class="logo" href="">logins</a>
    </header>
    <p>Nome:</p>
    <input v-model="nome" />
    <p>CPF:</p>
    <input type="text" class="form-control cpf-mask" placeholder="">
    <p>Email:</p>
    <input type="email" v-model="email" />
    <p>Telefone:</p>
    <input type="text" class="form-control phone-ddd-mask" placeholder="">
    <P>Data de nascimento:</P>
    <input type="text" class="form-control date-mask" id="example-input-1" placeholder="" maxlength="10"
      autocomplete="off">
    <p>Endereço:</p>
    <p><select>
        <option value="0" selected="selected">CIDADE</option>
        <option value="10167">Águas Frias</option>
        <option value="10180">Anchita</option>
        <option value="6551">Aquarari</option>
        <option value="6550">Ararangua</option>
        <option value="6544">Balneário Camburiú</option>
        <option value="6117">Balneário Piçarras</option>
        <option value="10182">Barra Bonita</option>
        <option value="10183">Belmonte</option>
        <option value="6541">Biguaçu</option>
        <option value="6540">Blumenal</option>
        <option value="10165">Bombinhas</option>
        <option value="6536">Brusque</option>
        <option value="6535">Caçador</option>
        <option value="6213">Caibi</option>
        <option value="6212">Camburiú</option>
        <option value="6208">Campos Novos</option>
        <option value="6206">Canoinhas</option>
        <option value="7397">Capivari de Baixo</option>
        <option value="10166">Caxambu do Sul</option>
        <option value="6202">Chapecó</option>
        <option value="7773">Cocal do Sul</option>
        <option value="6201">Concordia</option>
        <option value="6045">Correia Pinto</option>
        <option value="10162">Corupá</option>
        <option value="6198">Criciuma</option>
        <option value="6197">Cunha Pora</option>
        <option value="6196">Curitibanos</option>
        <option value="6195">Descanso</option>
        <option value="6194">Dionisio Cerqueira</option>
        <option value="10184">Flor do Sertão</option>
        <option value="6190">Florianópolis</option>
        <option value="9999">Forquilha</option>
        <option value="6187">Governador Celso Ramos</option>
        <option value="6181">Guabiruba</option>
        <option value="6180">Guaraciaba</option>
        <option value="6179">Guaramirim</option>
        <option value="6178">Guaruja do Sul</option>
        <option value="6174">Icara</option>
        <option value="6173">Ilhota</option>
        <option value="5588">Ipora do Oeste</option>
        <option value="5587">Iraceminha</option>
        <option value="6162">Itajaí</option>
        <option value="10160">Itapema</option>
        <option value="6155">Jaraguá do Sul</option>
        <option value="6154">Joaçaba</option>
        <option value="6153">Joinville</option>
        <option value="6151">Lages</option>
        <option value="6150">Laguna</option>
        <option value="6143">Mafra</option>
        <option value="6999">Maracajá</option>
        <option value="6140">Maravilha</option>
        <option value="6136">Modelo</option>
        <option value="6135">Mondai</option>
        <option value="6132">Navegantes</option>
        <option value="6131">Nova Erechim</option>
        <option value="6130">Nova Trento</option>
        <option value="6128">Orleans</option>
        <option value="6126">Palhoça</option>
        <option value="6125">Palma Sola</option>
        <option value="10175">Palmitos</option>
        <option value="10185">Paraíso</option>
        <option value="6120">Penha</option>
        <option value="6116">Pinhalzinho</option>
        <option value="6110">Porto Belo</option>
        <option value="6109">Porto União</option>
        <option value="6097">Rio do Sul</option>
        <option value="10163">Rio Negrinho</option>
        <option value="10187">Riqueza</option>
        <option value="6093">Romelandia</option>
        <option value="10188">Santa Helena</option>
        <option value="10164">Santa Terezinha do Progresso</option>
        <option value="6088">Santo Amaro da Imperatiz</option>
        <option value="6087">São Bento do Sul</option>
        <option value="7012">São Carlos</option>
        <option value="6083">São Fransquico do Sul</option>
        <option value="6082">São João Batista</option>
        <option value="10189">São João do Oeste</option>
        <option value="6080">São Joaquim</option>
        <option value="6079">São José</option>
        <option value="6078">São Jose do Cedro</option>
        <option value="6076">São Lourenço do Oeste</option>
        <option value="6073">São Miguel do Oeste</option>
        <option value="6072">Saudades</option>
        <option value="6071">Schreder</option>
        <option value="10176">Serra Alta</option>
        <option value="6068">Sombrio</option>
        <option value="10177">Sul Brasil</option>
        <option value="10191">Tigrinhos</option>
        <option value="6065">Tijucas</option>
        <option value="6059">Tubarão</option>
        <option value="10192">Tunópilis</option>
        <option value="10178">União do Oeste</option>
        <option value="6056">Urussanga</option>
        <option value="6053">Videira</option>
        <option value="6051">Xanxere</option>
        <option value="6050">Xavantina</option>
        <option value="6049">Xaxim</option>
      </select>
      <select class="form-control form-control-lg">
        <option value="0" selected="selected">ESTADOS</option>
        <option>AC</option>
        <option>AL</option>
        <option>AP</option>
        <option>AM</option>
        <option>BA</option>
        <option>CE</option>
        <option>DF</option>
        <option>ES</option>
        <option>GO</option>
        <option>MA</option>
        <option>MT</option>
        <option>MS</option>
        <option>MG</option>
        <option>PA</option>
        <option>PB</option>
        <option>PR</option>
        <option>PE</option>
        <option>PI</option>
        <option>RJ</option>
        <option>RN</option>
        <option>RS</option>
        <option>RO</option>
        <option>RR</option>
        <option>SC</option>
        <option>SP</option>
        <option>SE</option>
        <option>TO</option>
      </select>
    </p>
    <p>Bairro:</p>
    <p><input type="text" class="form-control form-control-lg" placeholder=""></p>
    <p>Rua/Avenida/Br:</p>
    <p><input type="text" class="form-control form-control-lg" placeholder=""></p>
    <p>Número da casa/apartamento:</p>
    <p><input type="text" class="from-control" placeholder=""></p>
    <p>Senha:</p>
    <input type="password" v-model="senha" />
    <p>Confirma senha:</p>
    <input type="password" v-model="confirmaSenha" />
    <form>
      <div class="form-check mb-3">
        <label class="form-check-label">
          <p>
            <input class="form-check-input" type="checkbox" name="remember"> Lembrar dados
          </p>
        </label>
      </div>
      <div class="li">
        <td data-align="center"
          style="text-align:-khtml-center;text-align:-moz-center;text-align:-webkit-center;height:25px"
          class="gx-tab-padding-fix-1   ">&nbsp;<span class="CheckBox"
            style="font-family:'Microsoft Sans Serif'; font-size:12.0pt; font-weight:normal; font-style:normal;"><input
              type="checkbox" id="vISCONFIRMED" name="vISCONFIRMED" value=""
              onfocus="gx.evt.onfocus(this, 49,'',false,'0002',0)"
              onclick="gx.fn.checkboxClick(49, this, 'true', 'false','');gx.evt.onchange(this, event);"
              onblur=";gx.evt.onblur(this,49);" data-gx-context="[&quot;&quot;,false]"><label data-gx-checkbox-title=""
              for="vISCONFIRMED">Li e concordo com todos os termos e condições.</label>
          </span>
        </td>
      </div>
      <button type="submit" class="btn btn-primary">Confirma</button>
    </form>
  </div>
</template>

<style>
.app {
  margin-left: auto;
  margin-right: auto;
}

button {
  background-color: rgb(129, 255, 158);
  text-align: center;
  border-radius: 7.5px;
  box-shadow: 3px 3px 1px rgb(128, 21, 43);
  transition: transform 1s;
}

nav {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  align-items: flex-start;
  justify-content: center;
}

button:hover,
button:focus {
  background: rgb(98, 255, 135);
  transform: translateX(12px) scale(1.2);
  box-shadow: 4px 4px 2.5px rgb(128, 21, 43);
}


input {
  border-radius: 5px;
  margin-top: 5px;
  box-shadow: 4px 2px 1.5px rgb(128, 21, 43);
}

p {
  font-style: italic;
  font-weight: bolder;
  color: rgb(255, 255, 255);
}

select {
  border-radius: 5px;
  margin-top: 5px;
  box-shadow: 4px 2px 1.5px rgb(128, 21, 43);
}

.li {
  margin-left: auto;
  margin-right: auto;
  font-style: italic;
  font-weight: bolder;
  color: rgb(255, 255, 255);
}

header {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  align-items: flex-start;
  justify-content: center;
  box-shadow: 4px 2px 1.5px rgb(128, 21, 43);
}
</style>