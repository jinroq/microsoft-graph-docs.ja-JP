---
title: Excel のブックとグラフの API の概要
description: Excel は、必要不可欠な生産性向上ツールです。 あらゆる業界と職務のユーザーが、あらゆる種類のデータを保存、追跡、操作するためのツールとして採用しています。 簡単なタスク追跡やデータ管理から複雑な計算や本格的なレポートに至るまで、あらゆる作業に使用されます。 Microsoft Graph で Excel REST API を使用して、データ、計算、レポート、およびダッシュボードの値を拡張できます。
localization_priority: Priority
author: lumine2008
ms.prod: excel
scenarios: getting-started
ms.openlocfilehash: 23f443766ba2d8539d2a4b79e5df379dce8c252d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793003"
---
# <a name="excel-workbooks-and-charts-api-overview"></a>Excel のブックとグラフの API の概要

Excel は、必要不可欠な生産性向上ツールです。 あらゆる業界と職務のユーザーが、あらゆる種類のデータを保存、追跡、操作するためのツールとして採用しています。 簡単なタスク追跡やデータ管理から複雑な計算や本格的なレポートに至るまで、あらゆる作業に使用されます。 Microsoft Graph で Excel REST API を使用して、データ、計算、レポート、およびダッシュボードの値を拡張できます。

> [!VIDEO https://www.youtube-nocookie.com/embed/I1rSkJww2Dk]

## <a name="why-integrate-with-excel"></a>Excel と統合する理由

Microsoft Graph を使用すると、OneDrive、SharePoint、またはその他のサポートされているストレージ プラットフォームに格納されている Excel ブックを、Web アプリケーションやモバイル アプリケーションで読み取ったり変更したりすることができます。

### <a name="perform-calculations"></a>計算の実行

ユーザーは、Excel 内で詳細かつ複雑な計算を簡単に実行できる点を非常に気に入っています。 今では、Excel の強力な計算エンジンにアクセスして瞬時に結果を得ることができます。 たとえば、住宅ローン計算アプリで元金、金利、支払回数を含む簡単な API 呼び出しを行うことにより、Excel の PMT 関数を利用できます。 Excel が難しい作業をすべて行い、瞬時に毎月の返済額を返します。 現在、300 以上の Excel ワークシート関数が利用可能であり、Excel でサポートされている広範囲の数式に完全にアクセスできます。 複雑なビジネス モデルを繰り返し再構築する必要はありません。 開発者は、簡単な API 呼び出しによってこれらの計算を瞬時に実行し、結果を取得するように Excel をプログラミングできます。

### <a name="generate-reports-and-analyze-results"></a>レポートの生成と結果の分析

Excel は、簡単なデータ テーブルから複雑で本格的なダッシュボードまでをカバーする柔軟なレポートおよび分析ツールです。 現在では、Excel のすべてのレポート機能への完全なアクセスが提供され、Excel は Office 365 内のオンライン レポート サービスになっています。 ユーザーが現在作成し、利用しているレポート作成シナリオをカスタム アプリに取り込み、本格的なグラフ作成や大量のデータ分析をインテリジェントに行うことで、Excel がこれらのカスタマイズされたエクスペリエンスにシームレスに融合されることを想像してみてください。

### <a name="store-and-track-data"></a>データの保存と追跡

Excel は、データを保存して追跡するための優れたツールでもあります。 情報がブックに保存されている場合、そのデータは Office 365 と統合されている任意のアプリで使用できます。 そのコンテンツをカスタム ソリューションで読み取り、それらのソリューションのデータ ストレージとして Excel を使用できます。

>**注:** Excel の REST API では、Office Open XML ファイル形式のブック (`.xlsx` 拡張子のブック) のみがサポートされています。 `.xls` 拡張子のブックはサポートされていません。 

### <a name="using-the-excel-rest-api"></a>Excel REST API の使用
Microsoft Graph を使用すると、OneDrive、SharePoint、またはその他のサポートされているストレージ プラットフォームに格納されている Excel ブックを、Web アプリケーションやモバイル アプリケーションで読み取ったり変更したりすることができます。`Workbook` (つまり Excel ファイル) リソースには、リレーションシップを介するその他のすべての Excel リソースが含まれています。ファイルの場所を URL で指定すれば、ドライブ API でブックにアクセスできます。例:

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`

ブックに対して作成、読み取り、更新、削除 (CRUD) 操作を実行するための標準 REST API を使用して、一連の Excel オブジェクト (テーブル、範囲、グラフなど) にアクセスできます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Excel API](/graph/api/resources/excel?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Excel API](/graph/api/resources/excel?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

* [Microsoft Graph で Excel のセッションを管理する](excel-manage-sessions.md)
* [Microsoft Graph を使用して Excel ブックに書き込む](excel-write-to-workbook.md)
* [Microsoft Graph で Excel のブック関数を使用する](excel-use-functions.md)
* [Microsoft Graph により Excel のある範囲の書式を更新する](excel-update-range-format.md)
* [Microsoft Graph により Excel のグラフ イメージを表示する](excel-display-chart-image.md)
* [Excel REST API を使用する](/graph/api/resources/excel?view=graph-rest-1.0)
