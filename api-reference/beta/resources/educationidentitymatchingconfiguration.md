---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校データプロファイル id を照合するための設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内で更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6805fabd857e4e906fa095c372632edbcc27fa28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006389"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="438db-105">educationIdentityMatchingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="438db-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="438db-106">学校データプロファイル id を照合するための設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="438db-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="438db-107">これらの id には、学生と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="438db-107">These identities include students and teachers.</span></span> <span data-ttu-id="438db-108">これらの設定に基づいて、ユーザーがディレクトリ内で更新されます。</span><span class="sxs-lookup"><span data-stu-id="438db-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="438db-109">**注:** このリソースが選択されている場合、ユーザーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="438db-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="438db-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="438db-110">Properties</span></span>

| <span data-ttu-id="438db-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="438db-111">Property</span></span> | <span data-ttu-id="438db-112">型</span><span class="sxs-lookup"><span data-stu-id="438db-112">Type</span></span> | <span data-ttu-id="438db-113">説明</span><span class="sxs-lookup"><span data-stu-id="438db-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="438db-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="438db-114">**matchingOptions**</span></span> | <span data-ttu-id="438db-115">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="438db-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="438db-116">ユーザーアカウントと、更新するユーザーを一意に識別するために使用するオプションとの間のマッピング。</span><span class="sxs-lookup"><span data-stu-id="438db-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="438db-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="438db-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
