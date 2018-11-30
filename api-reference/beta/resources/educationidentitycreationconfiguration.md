---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073495"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="df83d-105">educationIdentityCreationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df83d-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="df83d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df83d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df83d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df83d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df83d-108">学校データ プロファイル id の作成時に設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="df83d-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="df83d-109">これらの id には、生徒と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="df83d-109">These identities include students and teachers.</span></span> <span data-ttu-id="df83d-110">これらの設定に基づいて、ユーザーがディレクトリに作成されます。</span><span class="sxs-lookup"><span data-stu-id="df83d-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="df83d-111">**注:** ディレクトリ同期がオンになって、設置型の間で同期する Active Directory と Azure Active Directory (AD の Azure) を使っている場合は、 [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)のリソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="df83d-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="df83d-112">[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="df83d-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df83d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df83d-113">Properties</span></span>

| <span data-ttu-id="df83d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df83d-114">Property</span></span> | <span data-ttu-id="df83d-115">型</span><span class="sxs-lookup"><span data-stu-id="df83d-115">Type</span></span> | <span data-ttu-id="df83d-116">説明</span><span class="sxs-lookup"><span data-stu-id="df83d-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="df83d-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="df83d-117">**userDomains**</span></span> | <span data-ttu-id="df83d-118">[educationIdentityDomain](educationidentitydomain.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="df83d-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="df83d-119">ユーザーの種類ごとに使用するドメインの一覧を設定します。</span><span class="sxs-lookup"><span data-stu-id="df83d-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="df83d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df83d-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```