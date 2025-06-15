<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator Matriks Advanced</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: #333;
        }

        .app-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            text-align: center;
            color: white;
            margin-bottom: 40px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .header p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        .app-selector {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .app-card {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            min-width: 250px;
            position: relative;
            overflow: hidden;
        }

        .app-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            transition: left 0.5s;
        }

        .app-card:hover::before {
            left: 100%;
        }

        .app-card:hover {
            transform: translateY(-10px) scale(1.05);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }

        .app-card.active {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .app-card h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .app-card p {
            color: #666;
            font-size: 0.9rem;
        }

        .app-card.active p {
            color: rgba(255,255,255,0.9);
        }

        .app-content {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            display: none;
        }

        .app-content.active {
            display: block;
            animation: fadeInUp 0.5s ease;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .matrix-input {
            display: grid;
            gap: 8px;
            justify-content: center;
            margin: 20px 0;
            background: #f8f9ff;
            padding: 20px;
            border-radius: 15px;
            border: 2px solid #e0e4ff;
        }

        .matrix-input.grid-2x2 { grid-template-columns: repeat(2, 60px); }
        .matrix-input.grid-3x3 { grid-template-columns: repeat(3, 60px); }
        .matrix-input.grid-4x4 { grid-template-columns: repeat(4, 60px); }
        .matrix-input.grid-5x5 { grid-template-columns: repeat(5, 60px); }

        .matrix-input input {
            width: 60px;
            height: 60px;
            text-align: center;
            font-size: 16px;
            border: 2px solid #ddd;
            border-radius: 10px;
            background: white;
            transition: all 0.3s ease;
        }

        .matrix-input input:focus {
            border-color: #667eea;
            box-shadow: 0 0 10px rgba(102, 126, 234, 0.3);
            outline: none;
        }

        .controls {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .btn {
            padding: 12px 24px;
            border: none;
            border-radius: 25px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            min-width: 120px;
        }

        .btn-primary {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.4);
        }

        .btn-secondary {
            background: #f8f9ff;
            color: #667eea;
            border: 2px solid #667eea;
        }

        .btn-secondary:hover {
            background: #667eea;
            color: white;
        }

        .size-selector {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }

        .size-btn {
            width: 40px;
            height: 40px;
            border: 2px solid #ddd;
            background: white;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }

        .size-btn.active {
            background: #667eea;
            color: white;
            border-color: #667eea;
        }

        .output {
            background: #f8f9ff;
            border: 2px solid #e0e4ff;
            border-radius: 15px;
            padding: 25px;
            margin-top: 30px;
            white-space: pre-wrap;
            font-family: 'Courier New', monospace;
            font-size: 14px;
            line-height: 1.6;
            max-height: 500px;
            overflow-y: auto;
        }

        .loading {
            text-align: center;
            color: #667eea;
            font-size: 18px;
            font-weight: 600;
            margin: 20px 0;
            display: none;
        }

        .loading.show {
            display: block;
            animation: pulse 1.5s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }

        .operation-selector {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
        }

        .operation-btn {
            padding: 10px 20px;
            border: 2px solid #ddd;
            background: white;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }

        .operation-btn.active {
            background: #667eea;
            color: white;
            border-color: #667eea;
        }

        .matrix-display {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .matrix-table {
            border-collapse: collapse;
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .matrix-table td {
            width: 50px;
            height: 50px;
            text-align: center;
            border: 1px solid #ddd;
            font-weight: 600;
            font-size: 16px;
        }

        .operator {
            font-size: 2rem;
            font-weight: bold;
            color: #667eea;
        }

        .result-highlight {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .result-highlight td {
            border-color: rgba(255,255,255,0.3);
        }

        @media (max-width: 768px) {
            .app-selector {
                flex-direction: column;
                align-items: center;
            }
            
            .matrix-input input {
                width: 50px;
                height: 50px;
                font-size: 14px;
            }
            
            .controls {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="app-container">
        <div class="header">
            <h1>🧮 Kalkulator Matriks Advanced</h1>
            <p>Aplikasi lengkap untuk operasi matriks dengan UI modern dan interaktif</p>
        </div>

        <div class="app-selector">
            <div class="app-card active" data-app="determinant">
                <h3>🔢 Determinan Matriks</h3>
                <p>Hitung determinan matriks 2x2 hingga 5x5 dengan metode ekspansi kofaktor dan Sarrus</p>
            </div>
            <div class="app-card" data-app="operations">
                <h3>➕ Operasi Matriks</h3>
                <p>Penjumlahan dan pengurangan matriks dengan tampilan visual yang menarik</p>
            </div>
        </div>

        <!-- Determinant Calculator -->
        <div class="app-content active" id="determinant-app">
            <h2 style="text-align: center; margin-bottom: 30px; color: #667eea;">🔢 Kalkulator Determinan Matriks</h2>
            
            <div style="text-align: center; margin-bottom: 20px;">
                <label style="font-weight: 600; margin-bottom: 10px; display: block;">Pilih Ukuran Matriks:</label>
                <div class="size-selector">
                    <button class="size-btn" data-size="2">2×2</button>
                    <button class="size-btn" data-size="3">3×3</button>
                    <button class="size-btn active" data-size="4">4×4</button>
                    <button class="size-btn" data-size="5">5×5</button>
                </div>
            </div>

            <div class="matrix-input grid-4x4" id="det-matrix-input"></div>

            <div class="controls">
                <button class="btn btn-primary" onclick="calculateDeterminant()">🧮 Hitung Determinan</button>
                <button class="btn btn-secondary" onclick="randomMatrix('det')">🎲 Acak Matriks</button>
                <button class="btn btn-secondary" onclick="clearMatrix('det')">🗑️ Bersihkan</button>
            </div>

            <div class="loading" id="det-loading">⏳ Menghitung determinan...</div>
            <div class="output" id="det-output"></div>
        </div>

        <!-- Matrix Operations -->
        <div class="app-content" id="operations-app">
            <h2 style="text-align: center; margin-bottom: 30px; color: #667eea;">➕ Operasi Matriks</h2>
            
            <div style="text-align: center; margin-bottom: 20px;">
                <label style="font-weight: 600; margin-bottom: 10px; display: block;">Pilih Ukuran Matriks:</label>
                <div class="size-selector">
                    <button class="size-btn" data-size="2" onclick="setOperationSize(2)">2×2</button>
                    <button class="size-btn active" data-size="3" onclick="setOperationSize(3)">3×3</button>
                    <button class="size-btn" data-size="4" onclick="setOperationSize(4)">4×4</button>
                    <button class="size-btn" data-size="5" onclick="setOperationSize(5)">5×5</button>
                </div>
            </div>

            <div style="text-align: center; margin-bottom: 20px;">
                <label style="font-weight: 600; margin-bottom: 10px; display: block;">Pilih Operasi:</label>
                <div class="operation-selector">
                    <button class="operation-btn active" data-op="add">➕ Penjumlahan</button>
                    <button class="operation-btn" data-op="subtract">➖ Pengurangan</button>
                </div>
            </div>

            <div style="display: flex; justify-content: center; gap: 30px; flex-wrap: wrap;">
                <div>
                    <h3 style="text-align: center; margin-bottom: 15px;">Matriks A</h3>
                    <div class="matrix-input grid-3x3" id="matrix-a-input"></div>
                </div>
                <div>
                    <h3 style="text-align: center; margin-bottom: 15px;">Matriks B</h3>
                    <div class="matrix-input grid-3x3" id="matrix-b-input"></div>
                </div>
            </div>

            <div class="controls">
                <button class="btn btn-primary" onclick="calculateOperation()">🧮 Hitung</button>
                <button class="btn btn-secondary" onclick="randomMatrix('ops')">🎲 Acak Kedua Matriks</button>
                <button class="btn btn-secondary" onclick="clearMatrix('ops')">🗑️ Bersihkan</button>
            </div>

            <div class="loading" id="ops-loading">⏳ Menghitung operasi...</div>
            <div id="ops-result"></div>
        </div>
    </div>

    <script>
        let currentApp = 'determinant';
        let detSize = 4;
        let opsSize = 3;
        let currentOperation = 'add';

        // App switching
        document.querySelectorAll('.app-card').forEach(card => {
            card.addEventListener('click', () => {
                const app = card.dataset.app;
                switchApp(app);
            });
        });

        function switchApp(app) {
            // Update cards
            document.querySelectorAll('.app-card').forEach(c => c.classList.remove('active'));
            document.querySelector(`[data-app="${app}"]`).classList.add('active');
            
            // Update content
            document.querySelectorAll('.app-content').forEach(c => c.classList.remove('active'));
            document.getElementById(`${app}-app`).classList.add('active');
            
            currentApp = app;
        }

        // Size selector for determinant
        document.querySelectorAll('#determinant-app .size-btn').forEach(btn => {
            btn.addEventListener('click', () => {
                const size = parseInt(btn.dataset.size);
                setDeterminantSize(size);
            });
        });

        function setDeterminantSize(size) {
            detSize = size;
            document.querySelectorAll('#determinant-app .size-btn').forEach(b => b.classList.remove('active'));
            document.querySelector(`#determinant-app [data-size="${size}"]`).classList.add('active');
            
            const input = document.getElementById('det-matrix-input');
            input.className = `matrix-input grid-${size}x${size}`;
            input.innerHTML = '';
            
            for (let i = 0; i < size * size; i++) {
                const inputEl = document.createElement('input');
                inputEl.type = 'number';
                inputEl.value = '0';
                inputEl.id = `det-cell-${i}`;
                input.appendChild(inputEl);
            }
        }

        function setOperationSize(size) {
            opsSize = size;
            document.querySelectorAll('#operations-app .size-btn').forEach(b => b.classList.remove('active'));
            document.querySelector(`#operations-app [data-size="${size}"]`).classList.add('active');
            
            ['matrix-a-input', 'matrix-b-input'].forEach(id => {
                const input = document.getElementById(id);
                input.className = `matrix-input grid-${size}x${size}`;
                input.innerHTML = '';
                
                for (let i = 0; i < size * size; i++) {
                    const inputEl = document.createElement('input');
                    inputEl.type = 'number';
                    inputEl.value = '0';
                    inputEl.id = `${id}-cell-${i}`;
                    input.appendChild(inputEl);
                }
            });
        }

        // Operation selector
        document.querySelectorAll('.operation-btn').forEach(btn => {
            btn.addEventListener('click', () => {
                currentOperation = btn.dataset.op;
                document.querySelectorAll('.operation-btn').forEach(b => b.classList.remove('active'));
                btn.classList.add('active');
            });
        });

        // Initialize
        setDeterminantSize(4);
        setOperationSize(3);

        function getMatrix(prefix, size) {
            const matrix = [];
            for (let i = 0; i < size; i++) {
                const row = [];
                for (let j = 0; j < size; j++) {
                    const value = parseInt(document.getElementById(`${prefix}-cell-${i * size + j}`).value) || 0;
                    row.push(value);
                }
                matrix.push(row);
            }
            return matrix;
        }

        function getMinor(matrix, row, col) {
            return matrix.filter((_, i) => i !== row).map(r => r.filter((_, j) => j !== col));
        }

        function determinant2x2(matrix) {
            return matrix[0][0] * matrix[1][1] - matrix[0][1] * matrix[1][0];
        }

        function sarrus3x3(m) {
            const a = m[0], b = m[1], c = m[2];
            const pos = a[0]*b[1]*c[2] + a[1]*b[2]*c[0] + a[2]*b[0]*c[1];
            const neg = a[2]*b[1]*c[0] + a[0]*b[2]*c[1] + a[1]*b[0]*c[2];
            return pos - neg;
        }

        function calculateDeterminantRecursive(matrix) {
            const size = matrix.length;
            
            if (size === 1) return matrix[0][0];
            if (size === 2) return determinant2x2(matrix);
            if (size === 3) return sarrus3x3(matrix);
            
            let det = 0;
            for (let j = 0; j < size; j++) {
                const minor = getMinor(matrix, 0, j);
                const minorDet = calculateDeterminantRecursive(minor);
                const cofactor = ((-1) ** j) * minorDet;
                det += matrix[0][j] * cofactor;
            }
            return det;
        }

        function calculateDeterminant() {
            const loading = document.getElementById('det-loading');
            const output = document.getElementById('det-output');
            
            loading.classList.add('show');
            output.innerHTML = '';

            setTimeout(() => {
                const matrix = getMatrix('det', detSize);
                let result = `🔢 PERHITUNGAN DETERMINAN MATRIKS ${detSize}×${detSize}\n`;
                result += '='.repeat(60) + '\n\n';
                
                result += 'Matriks Input:\n';
                for (let i = 0; i < detSize; i++) {
                    result += `[${matrix[i].map(val => val.toString().padStart(4)).join(' ')}]\n`;
                }
                result += '\n';

                if (detSize === 2) {
                    const det = determinant2x2(matrix);
                    result += 'Metode 2×2:\n';
                    result += `det = (${matrix[0][0]} × ${matrix[1][1]}) - (${matrix[0][1]} × ${matrix[1][0]})\n`;
                    result += `det = ${matrix[0][0] * matrix[1][1]} - ${matrix[0][1] * matrix[1][0]}\n`;
                    result += `det = ${det}\n`;
                } else if (detSize === 3) {
                    const det = sarrus3x3(matrix);
                    result += 'Metode Sarrus 3×3:\n';
                    const a = matrix[0], b = matrix[1], c = matrix[2];
                    const pos1 = a[0]*b[1]*c[2], pos2 = a[1]*b[2]*c[0], pos3 = a[2]*b[0]*c[1];
                    const neg1 = a[2]*b[1]*c[0], neg2 = a[0]*b[2]*c[1], neg3 = a[1]*b[0]*c[2];
                    result += `Diagonal kanan ke kiri: ${pos1} + ${pos2} + ${pos3} = ${pos1+pos2+pos3}\n`;
                    result += `Diagonal kiri ke kanan: ${neg1} + ${neg2} + ${neg3} = ${neg1+neg2+neg3}\n`;
                    result += `Determinan = ${pos1+pos2+pos3} - (${neg1+neg2+neg3}) = ${det}\n`;
                } else {
                    // Ekspansi kofaktor untuk 4×4 dan 5×5
                    result += `Metode Ekspansi Kofaktor (Baris Pertama):\n\n`;
                    let det = 0;
                    
                    for (let j = 0; j < detSize; j++) {
                        const minor = getMinor(matrix, 0, j);
                        const minorDet = calculateDeterminantRecursive(minor);
                        const cofactor = ((-1) ** j) * minorDet;
                        const contrib = matrix[0][j] * cofactor;
                        det += contrib;
                        
                        result += `Elemen A[0][${j}] = ${matrix[0][j]}\n`;
                        result += `Minor ${detSize-1}×${detSize-1}:\n`;
                        for (let row of minor) {
                            result += `[${row.map(val => val.toString().padStart(4)).join(' ')}]\n`;
                        }
                        result += `Determinan minor = ${minorDet}\n`;
                        result += `Kofaktor = (-1)^${j} × ${minorDet} = ${cofactor}\n`;
                        result += `Kontribusi: ${matrix[0][j]} × ${cofactor} = ${contrib}\n`;
                        result += '-'.repeat(40) + '\n';
                    }
                    result += `\nDeterminan Total = ${det}\n`;
                }

                const finalDet = calculateDeterminantRecursive(matrix);
                result += '\n' + '='.repeat(60) + '\n';
                result += `✅ HASIL AKHIR: ${finalDet}\n`;
                result += '='.repeat(60);

                output.innerHTML = result;
                loading.classList.remove('show');
            }, 800);
        }

        function calculateOperation() {
            const loading = document.getElementById('ops-loading');
            const resultDiv = document.getElementById('ops-result');
            
            loading.classList.add('show');
            resultDiv.innerHTML = '';

            setTimeout(() => {
                const matrixA = getMatrix('matrix-a-input', opsSize);
                const matrixB = getMatrix('matrix-b-input', opsSize);
                
                let result = [];
                for (let i = 0; i < opsSize; i++) {
                    result[i] = [];
                    for (let j = 0; j < opsSize; j++) {
                        if (currentOperation === 'add') {
                            result[i][j] = matrixA[i][j] + matrixB[i][j];
                        } else {
                            result[i][j] = matrixA[i][j] - matrixB[i][j];
                        }
                    }
                }

                const operatorSymbol = currentOperation === 'add' ? '+' : '-';
                const operationName = currentOperation === 'add' ? 'Penjumlahan' : 'Pengurangan';

                resultDiv.innerHTML = `
                    <h3 style="text-align: center; margin: 30px 0; color: #667eea;">Hasil ${operationName} Matriks</h3>
                    <div class="matrix-display">
                        ${createMatrixTable(matrixA, 'Matriks A')}
                        <div class="operator">${operatorSymbol}</div>
                        ${createMatrixTable(matrixB, 'Matriks B')}
                        <div class="operator">=</div>
                        ${createMatrixTable(result, 'Hasil', true)}
                    </div>
                `;

                loading.classList.remove('show');
            }, 500);
        }

        function createMatrixTable(matrix, title, isResult = false) {
            let html = `<div><h4 style="text-align: center; margin-bottom: 10px;">${title}</h4>`;
            html += `<table class="matrix-table ${isResult ? 'result-highlight' : ''}">`;
            for (let row of matrix) {
                html += '<tr>';
                for (let val of row) {
                    html += `<td>${val}</td>`;
                }
                html += '</tr>';
            }
            html += '</table></div>';
            return html;
        }

        function randomMatrix(type) {
            if (type === 'det') {
                for (let i = 0; i < detSize * detSize; i++) {
                    document.getElementById(`det-cell-${i}`).value = Math.floor(Math.random() * 21) - 10;
                }
            } else {
                for (let i = 0; i < opsSize * opsSize; i++) {
                    document.getElementById(`matrix-a-input-cell-${i}`).value = Math.floor(Math.random() * 21) - 10;
                    document.getElementById(`matrix-b-input-cell-${i}`).value = Math.floor(Math.random() * 21) - 10;
                }
            }
        }

        function clearMatrix(type) {
            if (type === 'det') {
                for (let i = 0; i < detSize * detSize; i++) {
                    document.getElementById(`det-cell-${i}`).value = '0';
                }
                document.getElementById('det-output').innerHTML = '';
            } else {
                for (let i = 0; i < opsSize * opsSize; i++) {
                    document.getElementById(`matrix-a-input-cell-${i}`).value = '0';
                    document.getElementById(`matrix-b-input-cell-${i}`).value = '0';
                }
                document.getElementById('ops-result').innerHTML = '';
            }
        }
    </script>
</body>
</html>
