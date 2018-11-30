---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。
ms.openlocfilehash: 018cd422b56724811e1913ff0e94aea16d7c68f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068806"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| ブール値 | この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用して ID トークンを要求できるかどうかを指定します。|
|enableAccessTokenIssuance| ブール値 | この web アプリケーションで、OAuth 2.0 の暗黙的なフローを使用してアクセス トークンを要求できるかどうかを指定します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
