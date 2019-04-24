---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a3561768e36fc63c779e19a9aa05863dd9af9315
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505495"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="8fd55-103">office365ActivationsUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fd55-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8fd55-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fd55-104">Properties</span></span>

| <span data-ttu-id="8fd55-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fd55-105">Property</span></span>             | <span data-ttu-id="8fd55-106">型</span><span class="sxs-lookup"><span data-stu-id="8fd55-106">Type</span></span>                                     | <span data-ttu-id="8fd55-107">説明</span><span class="sxs-lookup"><span data-stu-id="8fd55-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="8fd55-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="8fd55-108">reportRefreshDate</span></span>    | <span data-ttu-id="8fd55-109">Date</span><span class="sxs-lookup"><span data-stu-id="8fd55-109">Date</span></span>                                     | <span data-ttu-id="8fd55-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="8fd55-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="8fd55-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8fd55-111">userPrincipalName</span></span>    | <span data-ttu-id="8fd55-112">String</span><span class="sxs-lookup"><span data-stu-id="8fd55-112">String</span></span>                                   | <span data-ttu-id="8fd55-113">ユーザーのユーザープリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="8fd55-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="8fd55-114">UPN は、インターネット標準 RFC 822 に基づくユーザーのインターネットスタイルのログイン名です。</span><span class="sxs-lookup"><span data-stu-id="8fd55-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="8fd55-115">規則により、これはユーザーの電子メール名にマップする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fd55-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="8fd55-116">一般的な形式は、検証済みドメインのテナントのコレクションにドメインが存在する必要がある、エイリアス @ domain です。</span><span class="sxs-lookup"><span data-stu-id="8fd55-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="8fd55-117">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="8fd55-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="8fd55-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8fd55-118">displayName</span></span>          | <span data-ttu-id="8fd55-119">String</span><span class="sxs-lookup"><span data-stu-id="8fd55-119">String</span></span>                                   | <span data-ttu-id="8fd55-120">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="8fd55-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="8fd55-121">これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。</span><span class="sxs-lookup"><span data-stu-id="8fd55-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="8fd55-122">このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="8fd55-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="8fd55-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="8fd55-123">userActivationCounts</span></span> | <span data-ttu-id="8fd55-124">[userActivationCounts](../resources/useractivationcounts.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8fd55-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="8fd55-125">ユーザーの最新の製品ライセンス認証は、割り当てられたすべての製品タイプのすべてのプラットフォームでカウントされます。</span><span class="sxs-lookup"><span data-stu-id="8fd55-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fd55-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fd55-126">JSON representation</span></span>

<span data-ttu-id="8fd55-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fd55-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
