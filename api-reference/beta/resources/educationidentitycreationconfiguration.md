---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データプロファイル id の作成に関する設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e35eed699e1a1439fd94c251e560be902f96bd09
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340562"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="cc4e4-105">educationIdentityCreationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc4e4-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc4e4-106">学校データプロファイル id の作成に関する設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="cc4e4-107">これらの id には、学生と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-107">These identities include students and teachers.</span></span> <span data-ttu-id="cc4e4-108">これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="cc4e4-109">**注:** オンプレミスの Active directory と azure active directory (azure AD) との間でディレクトリ同期をオンにしている場合は、代わりに[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)リソースを使用します。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="cc4e4-110">[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cc4e4-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4e4-111">Properties</span></span>

| <span data-ttu-id="cc4e4-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4e4-112">Property</span></span> | <span data-ttu-id="cc4e4-113">型</span><span class="sxs-lookup"><span data-stu-id="cc4e4-113">Type</span></span> | <span data-ttu-id="cc4e4-114">説明</span><span class="sxs-lookup"><span data-stu-id="cc4e4-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cc4e4-115">**userdomains**</span><span class="sxs-lookup"><span data-stu-id="cc4e4-115">**userDomains**</span></span> | <span data-ttu-id="cc4e4-116">[educationIdentityDomain](educationidentitydomain.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc4e4-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="cc4e4-117">ユーザーの種類ごとに使用するドメインのリストを設定します。</span><span class="sxs-lookup"><span data-stu-id="cc4e4-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="cc4e4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc4e4-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
