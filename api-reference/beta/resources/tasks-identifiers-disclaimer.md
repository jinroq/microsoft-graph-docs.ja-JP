---
title: タスクの識別子
description: タスク内のオブジェクトの識別子は、サービスによって生成された文字列値です。 . 値は 28 文字以内であり、大文字小文字を区別します。 渡されると、サービスは、形式検証が失敗した場合、呼び出し元は応答が正しくない要求 (400) エラーこの問題を示す場合に識別子の単純な形式の検証を行います。 このエラーが発生すると、呼び出し元のアプリケーション内のバグは次のようを示します。
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527613"
---
# <a name="identifiers-in-tasks"></a>タスクの識別子

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

タスク内のオブジェクトの識別子は、サービスによって生成された文字列値です。 . 値は 28 文字以内であり、大文字小文字を区別します。 渡されると、サービスは、形式検証が失敗した場合、呼び出し元は応答が正しくない要求 (400) エラーこの問題を示す場合に識別子の単純な形式の検証を行います。 このエラーが発生すると、呼び出し元のアプリケーション内のバグは次のようを示します。

- 呼び出し元のアプリケーションが、大文字と小文字を区別しない文字列として識別子を処理した。タスクの識別子は大文字と小文字を区別します。
- 呼び出し元のアプリケーションが、識別子を切り詰めた。タスクの識別子の長さは、28 文字です。
- 呼び出し元のアプリケーションが、タスクのオブジェクトに対して識別子の値を生成しようとした。クライアントにより生成された識別子は許可されません。すべての識別子は、オブジェクトの作成時にサービスによって生成されます。

この検証は、**セキュリティ機能ではありません**。これは、通知されないと特定することが難しい、アプリケーション開発時によくある識別子関連の問題についてアプリケーションに通知することを目的としたものです。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
