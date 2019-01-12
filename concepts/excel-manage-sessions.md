---
title: Microsoft Graph によって Excel のセッションと永続化を管理する
description: アプリケーションで Excel API の呼び出しを 1 回以上行う必要がある場合は、セッションを作成し、要求ごとにセッション ID を渡す必要がります。 要求にセッション ID を含めると、Excel API を最も効率的な方法で使用できるようになります。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 151119a2a2861b64db126c8f49d0b916a6f563e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921690"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a>Microsoft Graph によって Excel のセッションと永続化を管理する

アプリケーションで Excel API の呼び出しを 1 回以上行う必要がある場合は、セッションを作成し、要求ごとにセッション ID を渡す必要がります。 要求にセッション ID を含めると、Excel API を最も効率的な方法で使用できるようになります。

Excel API は、次の 3 つのモードのいずれかで呼び出すことができます。

1. **永続セッション**: ブックに加えられたすべての変更がブックに永続化 (保存) されます。 これは、最も効率的でパフォーマンスの高い Excel API の使用方法です。
2. **非永続セッション**: API によって加えられた変更は元の場所に保存されません。 代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。 Excel のセッションの有効期限が切れると、変更は失われます。 分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるが、ドキュメントの状態に影響を与える必要がないアプリでは、このモードが便利です。
3. **セッションレス**: API の呼び出しでセッション ID を渡しません。Excel サーバーは、操作ごとにサーバーに保存されたブックのコピーを検索する必要があります。 これは、効率的な Excel API の呼び出し方法ではありませんが、ある種の独立した要求を行うのに適しています。

API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。

>**注:** セッション ヘッダーは Excel API が機能するために必要ではありません。しかし、パフォーマンスを向上させるためにセッション ヘッダーを使用することをお勧めします。セッション ヘッダーを使用しない場合は、API の呼び出し時に行われた変更がファイルに永続化_されます_。  

## <a name="next-step"></a>次のステップ
セッションの作成方法と使用方法については、[セッション作成のリファレンス トピック](/graph/api/workbook-createsession?view=graph-rest-1.0)を参照してください。

## <a name="see-also"></a>関連項目
* [Microsoft Graph を使用して Excel ブックに書き込む](excel-write-to-workbook.md)
* [Microsoft Graph で Excel のブック関数を使用する](excel-use-functions.md)
* [Microsoft Graph により Excel のある範囲の書式を更新する](excel-update-range-format.md)
* [Microsoft Graph により Excel のグラフ イメージを表示する](excel-display-chart-image.md)
* [Excel REST API を使用する](/graph/api/resources/excel?view=graph-rest-1.0)
