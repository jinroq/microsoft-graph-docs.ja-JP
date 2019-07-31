---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972678"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="c5d80-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5d80-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5d80-106">すべての学校データプロファイル id 同期構成の抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="c5d80-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="c5d80-107">派生クラスは、id を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="c5d80-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="c5d80-108">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5d80-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="c5d80-109">派生型</span><span class="sxs-lookup"><span data-stu-id="c5d80-109">Derived types</span></span>
| <span data-ttu-id="c5d80-110">型</span><span class="sxs-lookup"><span data-stu-id="c5d80-110">Type</span></span> | <span data-ttu-id="c5d80-111">説明</span><span class="sxs-lookup"><span data-stu-id="c5d80-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="c5d80-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c5d80-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="c5d80-113">この種類を使用して、Azure Active Directory (Azure AD) の既存のユーザーアカウントと照合します。</span><span class="sxs-lookup"><span data-stu-id="c5d80-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="c5d80-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c5d80-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="c5d80-115">この種類を使用して、Azure AD で新しいユーザーアカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5d80-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5d80-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5d80-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

