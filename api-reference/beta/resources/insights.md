---
title: 情報リソースの種類
description: 情報は、関係の高度な解析と機械学習技術を使用して計算です。 OneDrive ドキュメントがユーザーの周りのトレンド分析を識別するなど。
author: simonhult
ms.openlocfilehash: f3269134f4a80462359a11d603c3f843be0c62f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318600"
---
# <a name="insights-resource-type"></a>情報リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

情報は、関係の高度な解析と機械学習技術を使用して計算です。 OneDrive ドキュメントがユーザーの周りのトレンド分析を識別するなど。

次の Api では、情報が返されます。

- [Trending](insights-trending.md)のでは、OneDrive と SharePoint サイトのユーザーの周りのトレンド分析から、ドキュメントが返されます。
- [使用されている](insights-used.md)のでは、ドキュメントの表示し、ユーザーが変更を返します。 ビジネス、SharePoint、電子メールの添付ファイル、およびボックス、ドロップ ボックスや Google のドライブのようなソースからのリンクの添付ファイルとして開かれたの OneDrive で、ユーザーが使用するドキュメントが含まれます。
- [共有](insights-shared.md)では、ユーザーと共有するドキュメントを返します。 ドキュメント共有できる電子メールの添付ファイル、または OneDrive としてビジネスに送信した電子メールのリンクをします。

各情報が返されます、`resourceVisualization`と`resourceReference`複雑な値の種類 (CVT) です。 含まれているプロパティを次のように CVT の resourceVisualization`title`と`previewImageUrl`。 マイクロソフトは、Office の説明のような経験でファイルを表示するのに視覚エフェクトのプロパティを使用します。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ      | 型          | 説明  |
| ------------- |---------------| -------------|
| トレンド分析      | [Trending](insights-trending.md)コレクション       | トレンド分析ドキュメントを識別する計算の関係です。 OneDrive または SharePoint サイトでは、トレンドのドキュメントを格納できます。   |
| used      | コレクションの[使用](insights-used.md)       | ドキュメントを表示し、ユーザーによって変更を識別するリレーションシップが計算されます。 ビジネス、SharePoint、電子メールの添付ファイル、およびボックス、ドロップ ボックスや Google のドライブのようなソースからのリンクの添付ファイルとして開かれたの OneDrive で、ユーザーが使用するドキュメントが含まれます。  |
| shared        | [共有](insights-shared.md)コレクション       | ユーザーと共有するドキュメントを識別する計算の関係です。 ドキュメント共有できる電子メールの添付ファイル、または OneDrive としてビジネスに送信した電子メールのリンクをします。   |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```