---
layout: default
---

<style>
.page-tabs {
  display: flex;
  gap: 0;
  border-bottom: 2px solid #e1e4e8;
  margin-bottom: 2.5rem;
}

.tab-link {
  padding: 0.75rem 1.5rem;
  text-decoration: none;
  color: #586069;
  border-bottom: 3px solid transparent;
  transition: all 0.2s;
  font-weight: 500;
  font-size: 0.95rem;
}

.tab-link:hover {
  color: #0366d6;
}

.tab-link.active {
  color: #0366d6;
  border-bottom-color: #0366d6;
}

/* 필터 섹션 - 크기 축소 */
.filter-section {
  margin: 15px 0;
  padding: 12px 15px;
  background: #f6f8fa;
  border-radius: 6px;
  font-size: 0.85em;
}

/* 필터 그룹 - 간격 축소 */
.filter-group {
  margin: 8px 0;
  padding: 6px 0;
  border-bottom: 1px solid #e1e4e8;
}

.filter-group:last-child {
  border-bottom: none;
}

.filter-group:first-child {
  border-bottom: 2px solid #d1d5da;
  padding-bottom: 10px;
  margin-bottom: 12px;
}

.filter-group-title {
  font-size: 0.75em;
  font-weight: 600;
  color: #24292e;
  margin-bottom: 5px;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.tag-btn {
  padding: 3px 9px;
  margin: 2px;
  border: 1px solid #d1d5da;
  background: white;
  cursor: pointer;
  border-radius: 3px;
  font-size: 0.8em;
  transition: all 0.2s;
}

.tag-btn:hover {
  background: #f6f8fa;
  border-color: #0366d6;
}

.tag-btn.active { 
  background: #0366d6; 
  color: white; 
  border-color: #0366d6;
}

/* 논문 아이템 */
.pub-item { 
  margin: 25px 0; 
  padding: 20px 0; 
  border-bottom: 1px solid #eaecef;
  transition: opacity 0.3s;
}

.pub-item:last-child {
  border-bottom: none;
}

.pub-item h3 {
  margin: 0 0 12px 0;
  font-size: 1.1em;
  font-weight: 600;
  line-height: 1.4;
}

.pub-tags { 
  margin: 10px 0; 
}

.tag {
  display: inline-block;
  padding: 3px 10px;
  margin: 3px 5px 3px 0;
  border-radius: 4px;
  font-size: 0.75em;
  font-weight: 500;
}

/* Target 태그 색상 (파란 계열) */
.tag-Building { background: #e3f2fd; color: #1565c0; }
.tag-Road { background: #e1f5fe; color: #0277bd; }
.tag-Bridge { background: #e0f2f1; color: #00695c; }
.tag-Plant { background: #e8eaf6; color: #3949ab; }

/* Purpose 태그 색상 (주황/빨강 계열) */
.tag-Fire { background: #ffebee; color: #c62828; }
.tag-Safety { background: #fff3e0; color: #e65100; }
.tag-Automation { background: #fce4ec; color: #c2185b; }
.tag-Information { background: #f3e5f5; color: #7b1fa2; }
.tag-Education { background: #ede7f6; color: #512da8; }

/* Method 태그 색상 (녹색/보라 계열) */
.tag-BIM { background: #e8f5e9; color: #2e7d32; }
.tag-SNA { background: #f1f8e9; color: #558b2f; }
.tag-AI { background: #fff9c4; color: #f57f17; }
.tag-LLM { background: #f3e5f5; color: #6a1b9a; }
.tag-LMM { background: #ede7f6; color: #4527a0; }
.tag-Simulation { background: #e0f7fa; color: #00838f; }
.tag-Ontology { background: #e0f2f1; color: #00695c; }
.tag-Blockchain { background: #e3f2fd; color: #0d47a1; }

/* Type & Language 태그 색상 */
.tag-type { background: #eceff1; color: #37474f; }
.tag-lang { background: #fff8e1; color: #f57f17; }

.pub-item p {
  margin: 8px 0;
  color: #586069;
  font-size: 0.95em;
}

.pub-item a {
  color: #0366d6;
  text-decoration: none;
  font-size: 0.9em;
}

.pub-item a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .tag-btn {
    font-size: 0.75em;
    padding: 3px 8px;
  }
  
  .filter-group-title {
    font-size: 0.7em;
  }
  
  .filter-section {
    padding: 10px;
  }
}
</style>

<div class="page-tabs">
  <a href="./index.html" class="tab-link active">Home</a>
  <a href="./research.html" class="tab-link">Research</a>
  <a href="./teaching.html" class="tab-link">Teaching</a>
  <a href="./education.html" class="tab-link">Education</a>
</div>

Research interests: BIM, LLM/LMM, Construction Automation, and AI applications in Engineering.

# Publications

<div class="filter-section">
  <!-- All 버튼 -->
  <div class="filter-group">
    <button class="tag-btn active" data-tag="all" data-group="all">All</button>
  </div>

  <!-- Target 필터 그룹 -->
  <div class="filter-group">
    <div class="filter-group-title">Target</div>
    <button class="tag-btn" data-tag="Building" data-group="target">Building</button>
    <button class="tag-btn" data-tag="Road" data-group="target">Road</button>
    <button class="tag-btn" data-tag="Bridge" data-group="target">Bridge</button>
    <button class="tag-btn" data-tag="Plant" data-group="target">Plant</button>
  </div>

  <!-- Purpose 필터 그룹 -->
  <div class="filter-group">
    <div class="filter-group-title">Purpose</div>
    <button class="tag-btn" data-tag="Fire" data-group="purpose">Fire Safety</button>
    <button class="tag-btn" data-tag="Safety" data-group="purpose">Safety</button>
    <button class="tag-btn" data-tag="Automation" data-group="purpose">Automation</button>
    <button class="tag-btn" data-tag="Information" data-group="purpose">Information</button>
    <button class="tag-btn" data-tag="Education" data-group="purpose">Education</button>
  </div>

  <!-- Method 필터 그룹 -->
  <div class="filter-group">
    <div class="filter-group-title">Method</div>
    <button class="tag-btn" data-tag="BIM" data-group="method">BIM</button>
    <button class="tag-btn" data-tag="SNA" data-group="method">SNA</button>
    <button class="tag-btn" data-tag="AI" data-group="method">AI</button>
    <button class="tag-btn" data-tag="LLM" data-group="method">LLM</button>
    <button class="tag-btn" data-tag="LMM" data-group="method">LMM</button>
    <button class="tag-btn" data-tag="Simulation" data-group="method">Simulation</button>
    <button class="tag-btn" data-tag="Ontology" data-group="method">Ontology</button>
    <button class="tag-btn" data-tag="Blockchain" data-group="method">Blockchain</button>
  </div>

  <!-- Type 필터 그룹 -->
  <div class="filter-group">
    <div class="filter-group-title">Type</div>
    <button class="tag-btn" data-tag="Journal" data-group="type">Journal</button>
    <button class="tag-btn" data-tag="Proceeding" data-group="type">Proceeding</button>
  </div>

  <!-- Language 필터 그룹 -->
  <div class="filter-group">
    <div class="filter-group-title">Language</div>
    <button class="tag-btn" data-tag="EN" data-group="language">EN</button>
    <button class="tag-btn" data-tag="KO" data-group="language">KO</button>
  </div>
</div>

<div class="publications">
  <div class="pub-item" data-tags="Plant,Safety,LLM,Ontology" data-type="Journal" data-lang="EN">
    <h3>Hierarchical Large Language Model and Semantic Web Rule Language Integration for Scalable and Consistent Ontology Expansion Enabling Automated Safety Compliance Checking</h3>
    <div class="pub-tags">
      <span class="tag tag-Plant">Plant</span>
      <span class="tag tag-Safety">Safety</span>
      <span class="tag tag-LLM">LLM</span>
      <span class="tag tag-Ontology">Ontology</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Engineering Applications of Artificial Intelligence</em>, 2026</p>
    <a href="Under review" target="_blank">Under review</a>
  </div>

  <div class="pub-item" data-tags="Building,BIM,Information" data-type="Journal" data-lang="EN">
    <h3>Automated Conversion and Semantic Gap Filling of Material Layer Annotations from CAD Drawings to Semantically Rich BIM Objects</h3>
    <div class="pub-tags">
      <span class="tag tag-Building">Building</span>
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-Information">Information</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Advanced Engineering Informatics</em>, 2026</p>
    <a href="Accepted" target="_blank">Accepted</a>
  </div>

  <div class="pub-item" data-tags="AI,Education" data-type="Journal" data-lang="KO">
    <h3>Development of Digital Competency Index and Analysis of Competency Changes in Korean College Architecture Curriculum - A Comparative Study of 2018 and 2025 -</h3>
    <div class="pub-tags">
      <span class="tag tag-AI">AI</span>
      <span class="tag tag-Education">Education</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of the Architectural Institute of Korea Structure & Construction</em>, 2025</p>
    <a href="Accepted" target="_blank">Accepted</a>
  </div>

  <div class="pub-item" data-tags="LMM,Safety" data-type="Journal" data-lang="EN">
    <h3>Automated Analysis of Construction Safety Accident Videos using a Large Multimodal Model and Graph Retrieval-Augmented Generation</h3>
    <div class="pub-tags">
      <span class="tag tag-LMM">LMM</span>
      <span class="tag tag-Safety">Safety</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Automation in Construction</em>, 2025</p>
    <a href="https://doi.org/10.1016/j.autcon.2025.106363" target="_blank">DOI: 10.1016/j.autcon.2025.106363</a>
  </div>

  <div class="pub-item" data-tags="Building,Education,BIM,Information,LLM" data-type="Journal" data-lang="EN">
    <h3>Effectiveness of Retrieval Augmented Generation-Based Large Language Models for Generating Construction Safety Information</h3>
    <div class="pub-tags">
      <span class="tag tag-LLM">LLM</span>
      <span class="tag tag-Safety">Safety</span>
      <span class="tag tag-Information">Information</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Automation in Construction</em>, 2025</p>
    <a href="https://doi.org/10.1016/j.autcon.2024.105926" target="_blank">DOI: 10.1016/j.autcon.2024.105926</a>
  </div>

  <div class="pub-item" data-tags="Blockchain" data-type="Journal" data-lang="KO">
    <h3>Research and Prototype Development on Enhancing Building Inspection Reliability using Dependency Graphs and Blockchain - Focused on Structural Inspection</h3>
    <div class="pub-tags">
      <span class="tag tag-Blockchain">Blockchain</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of the Korea Academia-Industrial cooperation Society</em>, 2025</p>
    <a href="https://doi.org/10.5762/KAIS.2025.26.10.391" target="_blank">DOI: 10.5762/KAIS.2025.26.10.391</a>
  </div>

  <div class="pub-item" data-tags="BIM" data-type="Proceeding" data-lang="EN">
    <h3>Filling in Missing Material Layer Information for Generating Wall and Slab Object Libraies from Drawing</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-type">Proceeding</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>2025 European Conference on Computing in Construction/ CIB W78 Conference on IT in Construction, July 14-17 2025 Porto Portugal</em>, 2025</p>
  </div>

  <div class="pub-item" data-tags="Safety" data-type="Journal" data-lang="EN">
    <h3>Enhancing Construction Managers' Risk Perception and Lowering Risk Tolerance toward Unsafe Behaviors Through Experiential Safety Training</h3>
    <div class="pub-tags">
      <span class="tag tag-Safety">Safety</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Journal of Management in Engineering</em>, 2024</p>
    <a href="https://doi.org/10.1061/JMENEA.MEENG-6283" target="_blank">DOI: 10.1061/JMENEA.MEENG-6283</a>
  </div>

  <div class="pub-item" data-tags="Road,Information" data-type="Journal" data-lang="EN">
    <h3>Exploring the Long-Term Impact of Preventive Road Treatments on Municipal Highways</h3>
    <div class="pub-tags">
      <span class="tag tag-Road">Road</span>
      <span class="tag tag-Information">Information</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Journal of Management in Engineering</em>, 2024</p>
    <a href="https://doi.org/10.1061/JMENEA.MEENG-5885" target="_blank">DOI: 10.1061/JMENEA.MEENG-5885</a>
  </div>

  <div class="pub-item" data-tags="Safety" data-type="Journal" data-lang="KO">
    <h3>Impact of Construction Safety Managers and Project Characteristics on Air Conditioning Installation Safety Scores</h3>
    <div class="pub-tags">
      <span class="tag tag-Safety">Safety</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of The Korea Institute of Building Construction</em>, 2024</p>
    <a href="https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003088534" target="_blank">DOI: 10.5345/JKIBC.2024.24.3.381</a>
  </div>
 
  <div class="pub-item" data-tags="BIM" data-type="Journal" data-lang="KO">
    <h3>BIM Performance Evaluation Method based on Post-Construction Evaluation</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of the Korea Academia-Industrial cooperation Society</em>, 2024</p>
    <a href="https://doi.org/10.5762/KAIS.2024.25.5.527" target="_blank">DOI: 10.5762/KAIS.2024.25.5.527</a>
  </div>

  <div class="pub-item" data-tags="Blockchain" data-type="Proceeding" data-lang="EN">
    <h3>Enhancing User-Participatory Processes in Road Pavement Defect Management through Blockchain Integration</h3>
    <div class="pub-tags">
      <span class="tag tag-Blockchain">Blockchain</span>
      <span class="tag tag-type">Proceeding</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>ASCE International Conference on Computing in Civil Engineering, July 28-31 2024 Pittsburgh, Pennsylvania, US</em>, 2024</p>
  </div>

  <div class="pub-item" data-tags="Road" data-type="Proceeding" data-lang="EN">
    <h3>Evaluating the Economic Impact of Preventive Treatment Strategies for Municipal Highways</h3>
    <div class="pub-tags">
      <span class="tag tag-Road">Road</span>
      <span class="tag tag-type">Proceeding</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>ASCE International Conference on Computing in Civil Engineering 2023 June 25–28, 2023, Corvallis, Oregon, US</em>, 2023</p>
  </div>

  <div class="pub-item" data-tags="BIM" data-type="Journal" data-lang="EN">
    <h3>Information Requirements for Managing Higher Education Facilities Using Building Information Modeling: Triangular Study of US and Korean Cases</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Journal of Computing in Civil Engineering</em>, 2021</p>
    <a href="https://doi.org/10.1061/(ASCE)CP.1943-5487.0000989" target="_blank">DOI: 10.1061/(ASCE)CP.1943-5487.0000989</a>
  </div>

  <div class="pub-item" data-tags="BIM,Education" data-type="Journal" data-lang="EN">
    <h3>An Analysis of BIM Jobs and Competencies based on the Use of Terms in the Industry</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-Education">Education</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Automation in Construction</em>, 2017</p>
    <a href="https://doi.org/10.1016/j.autcon.2017.06.002" target="_blank">DOI: 10.1016/j.autcon.2017.06.002</a>
  </div>
    
  <div class="pub-item" data-tags="Information" data-type="Journal" data-lang="KO">
    <h3>TAM3-based Analysis of the Differences in the Attitude toward FMS between User Groups by Experience in Higher Education Facilities</h3>
    <div class="pub-tags">
      <span class="tag tag-Information">Information</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of the Architectural Institute of Korea Structure & Construction</em>, 2016</p>
    <a href="https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002084396" target="_blank">DOI: 10.5659/JAIK_SC.2016.32.2.51</a>
  </div>

  <div class="pub-item" data-tags="ACC" data-type="Proceeding" data-lang="EN">
    <h3>Can Experience Overcome the Cognitive Challenges in Drawing Based Design Review? — Design Review Experiments</h3>
    <div class="pub-tags">
      <span class="tag tag-ACC">ACC</span>
      <span class="tag tag-type">Proceeding</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Proceedings of the 16th International Conference on Construction Applications of Virtual Reality, 11-13 December 2016, HK</em>, 2016</p>
  </div>

  <div class="pub-item" data-tags="BIM" data-type="Journal" data-lang="EN">
    <h3>Requirements for Computational Rule Checking of Requests for Proposals (RFPs) for Building Designs in South Korea</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">EN</span>
    </div>
    <p><em>Advanced Engineering Informatics</em>, 2015</p>
    <a href="https://doi.org/10.1016/j.aei.2015.05.006" target="_blank">DOI: 10.1016/j.aei.2015.05.006</a>
  </div>

  <div class="pub-item" data-tags="BIM" data-type="Journal" data-lang="KO">
    <h3>A Study on the Development Direction and Priority of the BIM-Based Hospital Design Validation Technology</h3>
    <div class="pub-tags">
      <span class="tag tag-BIM">BIM</span>
      <span class="tag tag-type">Journal</span>
      <span class="tag tag-lang">KO</span>
    </div>
    <p><em>Journal of the Architectural Institute of Korea Structure & Construction</em>, 2013</p>
    <a href="https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART001783229" target="_blank">UCI : G704-A00167.2013.29.06.031</a>
  </div>
</div>

# Contact

**Email:** [aha0810@yonsei.ac.kr](mailto:aha0810@yonsei.ac.kr)  
**Phone:** +82-10-3193-9558  
**Affiliation:** Department of Architecture and Architectural Engineering, Yonsei University

<script>
document.addEventListener('DOMContentLoaded', function() {
  const buttons = document.querySelectorAll('.tag-btn');
  const items = document.querySelectorAll('.pub-item');
  
  // 그룹별 활성 필터 관리
  const activeFilters = {
    all: true,
    target: new Set(),
    purpose: new Set(),
    method: new Set(),
    type: new Set(),
    language: new Set()
  };
  
  buttons.forEach(btn => {
    btn.addEventListener('click', function() {
      const tag = this.dataset.tag;
      const group = this.dataset.group;
      
      // All 버튼 클릭 시
      if (group === 'all') {
        buttons.forEach(b => b.classList.remove('active'));
        this.classList.add('active');
        activeFilters.all = true;
        Object.keys(activeFilters).forEach(key => {
          if (key !== 'all') activeFilters[key].clear();
        });
        filterPublications();
        return;
      }
      
      // All 비활성화
      activeFilters.all = false;
      document.querySelector('[data-group="all"]').classList.remove('active');
      
      // 현재 버튼 토글
      if (this.classList.contains('active')) {
        this.classList.remove('active');
        activeFilters[group].delete(tag);
      } else {
        this.classList.add('active');
        activeFilters[group].add(tag);
      }
      
      // 모든 필터가 비어있으면 All 활성화
      const hasActiveFilters = Object.keys(activeFilters).some(key => 
        key !== 'all' && activeFilters[key].size > 0
      );
      
      if (!hasActiveFilters) {
        document.querySelector('[data-group="all"]').classList.add('active');
        activeFilters.all = true;
      }
      
      filterPublications();
    });
  });
  
  function filterPublications() {
    items.forEach(item => {
      if (activeFilters.all) {
        item.style.display = 'block';
        return;
      }
      
      const itemTags = item.dataset.tags.split(',');
      const itemType = item.dataset.type;
      const itemLang = item.dataset.lang;
      
      // 각 그룹별 매칭 검사 (그룹 내 OR, 그룹 간 AND)
      const matchTarget = activeFilters.target.size === 0 || 
        [...activeFilters.target].some(t => itemTags.includes(t));
      
      const matchPurpose = activeFilters.purpose.size === 0 || 
        [...activeFilters.purpose].some(t => itemTags.includes(t));
      
      const matchMethod = activeFilters.method.size === 0 || 
        [...activeFilters.method].some(t => itemTags.includes(t));
      
      const matchType = activeFilters.type.size === 0 || 
        activeFilters.type.has(itemType);
      
      const matchLanguage = activeFilters.language.size === 0 || 
        activeFilters.language.has(itemLang);
      
      // 모든 조건 만족 시 표시
      if (matchTarget && matchPurpose && matchMethod && matchType && matchLanguage) {
        item.style.display = 'block';
      } else {
        item.style.display = 'none';
      }
    });
  }
});
</script>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const currentPage = window.location.pathname;
  const tabs = document.querySelectorAll('.page-tabs .tab-link');
  
  tabs.forEach(tab => {
    if (tab.getAttribute('href').includes(currentPage.split('/').pop())) {
      tabs.forEach(t => t.classList.remove('active'));
      tab.classList.add('active');
    }
  });
});
</script>