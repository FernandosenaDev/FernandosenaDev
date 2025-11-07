<h1>software engineer</h1>

import matplotlib.pyplot as plt
import numpy as np

# Estilo mais clean para GitHub
plt.style.use('seaborn-v0_8')

# Dados
periodos = ['Sprint 1', 'Sprint 2', 'Sprint 3', 'Sprint 4']
review_commits = [12, 18, 25, 30]
dev_commits = [30, 25, 18, 12]

fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(15, 5))

# Gráfico 1: Linhas
ax1.plot(periodos, review_commits, 'g-', label='Code Review', linewidth=3, marker='D')
ax1.plot(periodos, dev_commits, 'b-', label='Desenvolvimento', linewidth=3, marker='o')
ax1.set_title('🔁 Evolução de Commits')
ax1.set_ylabel('Commits por Sprint')
ax1.legend()
ax1.grid(True, alpha=0.3)

# Gráfico 2: Barras
width = 0.35
x = np.arange(len(periodos))
ax2.bar(x - width/2, review_commits, width, label='Code Review', color='#28a745', alpha=0.7)
ax2.bar(x + width/2, dev_commits, width, label='Desenvolvimento', color='#0366d6', alpha=0.7)
ax2.set_title('📈 Comparação por Sprint')
ax2.set_ylabel('Quantidade de Commits')
ax2.set_xticks(x)
ax2.set_xticklabels(periodos)
ax2.legend()

plt.suptitle('GitHub Metrics - Code Review vs Development', fontsize=16, fontweight='bold')
plt.tight_layout()
plt.show()
