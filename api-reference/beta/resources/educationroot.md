---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
ms.openlocfilehash: 01845df878d5e6a4fe01cb29f73d73b6980cfa9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067509"
---
# <a name="educationroot-resource-type"></a>educationRoot リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

`/education` 名前空間は、教育機関に固有の機能を公開します。 `/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。 教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| クラス コレクションに投稿して、新しい **educationClass** を作成します。|
|[List classes](../api/educationroot-list-classes.md) |[educationClass](educationclass.md) コレクション| **educationClass** オブジェクト コレクションを取得します。|
|[Create educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| 学校コレクションに投稿して、新しい **educationSchool** を作成します。|
|[List schools](../api/educationroot-list-schools.md) |[educationSchool](educationschool.md) コレクション| **educationSchool** オブジェクト コレクションを取得します。|
|[Create educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| ユーザー コレクションに投稿して、新しい **educationUser** を作成します。|
|[List users](../api/educationroot-list-users.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) コレクション| 読み取り専用。Null 許容型。|
|me|[educationUser](educationuser.md)| 読み取り専用。Null 許容型。|
|schools|[educationSchool](educationschool.md) コレクション| 読み取り専用。Null 許容型。|
|users|[educationUser](educationuser.md) コレクション| 読み取り専用。Null 許容型。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->