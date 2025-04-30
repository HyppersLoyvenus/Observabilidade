# Observabilidade
Aula sobre observabilidade de um banco de dados postgres com o prometheus e grafana (29/04/2025)

## Como Utilizar

Para configurar e executar toda a stack de observabilidade, siga os passos abaixo:

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/HyppersLoyvenus/Observabilidade.git
   cd Observabilidade
   ```

2. **Construa e execute os serviços**:
   ```bash
   docker-compose up --build -d
   ```

3. **Acesse os serviços**:
   - PostgreSQL: Conecte-se ao banco de dados usando o cliente de sua preferência (ex: Dbeaver);
   - Prometheus: Acesse a interface do Prometheus em `http://localhost:9090`;
   - Grafana: Acesse a interface do Grafana em `http://localhost:3000` (as credenciais padrão são `admin`/`admin`);
   - No Grafana: Clique no icone ao lado esquerdo e vá em `Data sources` - `add new data source` - selecione o prometheus e em connection digite: `http://prometheus:9090`;
   - Assim você já podera criar um dashboard e observar seu banco.
