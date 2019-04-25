---
title: タスクの識別子
description: タスク内のオブジェクトの識別子は、サービスによって生成された文字列値です。 . 値の長さは28文字で、大文字と小文字は区別されます。 として渡された場合、サービスは識別子の簡単な形式の検証を実行します。形式の検証が失敗した場合、発信者はこの問題を示す無効な要求 (400) のエラー応答を受信します。 このエラーは、次のような呼び出し元のアプリケーションにバグがあることを示しています。
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583225"
---
# <a name="identifiers-in-tasks"></a>タスクの識別子

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

タスク内のオブジェクトの識別子は、サービスによって生成された文字列値です。 . 値の長さは28文字で、大文字と小文字は区別されます。 として渡された場合、サービスは識別子の簡単な形式の検証を実行します。形式の検証が失敗した場合、発信者はこの問題を示す無効な要求 (400) のエラー応答を受信します。 このエラーは、次のような呼び出し元のアプリケーションにバグがあることを示しています。

- 呼び出し元のアプリケーションは、大文字と小文字を区別しない文字列として識別子を処理しました。 タスクの識別子では大文字と小文字が区別されます。
- 呼び出し元アプリケーションが識別子を切り捨てました。 タスクの識別子は、28文字の長さです。
- 呼び出し元のアプリケーションがタスクのオブジェクトの識別子値を生成しようとしました。 クライアントによって生成された識別子は受け付けられません。 すべての識別子は、オブジェクトの作成時にサービスによって生成されます。

この検証は**セキュリティ機能ではありません**。 これは、アプリケーションを開発する際に、アプリケーションについての一般的な識別子に関する問題についてのみ通知することを目的としています。これは、それ以外の場合はわかりにくいものです。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
