---
title: roleManagement リソースの種類
description: RBAC 役割管理リソース
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bd4e1eefeae819d37630a7faf4fbb1f6d1a5124c
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437819"
---
# <a name="rolemanagement-resource-type"></a>roleManagement リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 365 RBAC 役割管理エンティティ。 RBAC プロバイダーから表面化したロール定義およびロール割り当てへのアクセスを提供します。 現時点では、ディレクトリプロバイダーのみがサポートされています。 詳細については、「 [Azure Active Directory での管理者の役割のアクセス許可](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-assign-admin-roles)」を参照してください。

## <a name="methods"></a>メソッド

None

## <a name="properties"></a>プロパティ

なし

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|名簿|[rbacApplication](rbacapplication.md)| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

None

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
