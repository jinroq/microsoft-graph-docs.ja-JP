---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ee9f58c2f69882361ee105a1d7531bb5756e165
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977550"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="cedd7-105">educationIdentityMatchingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cedd7-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="cedd7-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cedd7-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cedd7-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cedd7-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cedd7-108">学校のデータのプロファイルの id を一致させるための設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="cedd7-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="cedd7-109">これらの id には、生徒と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cedd7-109">These identities include students and teachers.</span></span> <span data-ttu-id="cedd7-110">これらの設定に基づいて、ユーザーがディレクトリで更新されます。</span><span class="sxs-lookup"><span data-stu-id="cedd7-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="cedd7-111">**注:** このリソースが選択されている場合は、ユーザーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="cedd7-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="cedd7-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cedd7-112">Properties</span></span>

| <span data-ttu-id="cedd7-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cedd7-113">Property</span></span> | <span data-ttu-id="cedd7-114">種類</span><span class="sxs-lookup"><span data-stu-id="cedd7-114">Type</span></span> | <span data-ttu-id="cedd7-115">説明</span><span class="sxs-lookup"><span data-stu-id="cedd7-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cedd7-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="cedd7-116">**matchingOptions**</span></span> | <span data-ttu-id="cedd7-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cedd7-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="cedd7-118">ユーザー アカウントを更新するユーザーを一意に識別に使用するオプションの間のマッピングです。</span><span class="sxs-lookup"><span data-stu-id="cedd7-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cedd7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cedd7-119">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
