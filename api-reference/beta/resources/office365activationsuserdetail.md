---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 9cf0f7f841584654176c0069fb0403a86615bfd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068650"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="82f45-103">office365ActivationsUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82f45-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="82f45-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82f45-104">Properties</span></span>

| <span data-ttu-id="82f45-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82f45-105">Property</span></span>             | <span data-ttu-id="82f45-106">型</span><span class="sxs-lookup"><span data-stu-id="82f45-106">Type</span></span>                                     | <span data-ttu-id="82f45-107">説明</span><span class="sxs-lookup"><span data-stu-id="82f45-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="82f45-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="82f45-108">reportRefreshDate</span></span>    | <span data-ttu-id="82f45-109">Date</span><span class="sxs-lookup"><span data-stu-id="82f45-109">Date</span></span>                                     | <span data-ttu-id="82f45-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="82f45-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="82f45-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82f45-111">userPrincipalName</span></span>    | <span data-ttu-id="82f45-112">String</span><span class="sxs-lookup"><span data-stu-id="82f45-112">String</span></span>                                   | <span data-ttu-id="82f45-113">ユーザー プリンシパル名 (UPN) のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="82f45-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="82f45-114">UPN は、インターネット標準の RFC 822 に基づくユーザーに対して、インターネット スタイルのログイン名です。</span><span class="sxs-lookup"><span data-stu-id="82f45-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="82f45-115">規則では、これはユーザーの電子メール名にマップする必要があります。</span><span class="sxs-lookup"><span data-stu-id="82f45-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="82f45-116">一般的な形式は、ドメインをドメインの検証済みのテナントのコレクション内に存在する必要があります、alias@domain、です。</span><span class="sxs-lookup"><span data-stu-id="82f45-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="82f45-117">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="82f45-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="82f45-118">displayName</span><span class="sxs-lookup"><span data-stu-id="82f45-118">displayName</span></span>          | <span data-ttu-id="82f45-119">String</span><span class="sxs-lookup"><span data-stu-id="82f45-119">String</span></span>                                   | <span data-ttu-id="82f45-120">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="82f45-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="82f45-121">これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。</span><span class="sxs-lookup"><span data-stu-id="82f45-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="82f45-122">このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="82f45-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="82f45-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="82f45-123">userActivationCounts</span></span> | <span data-ttu-id="82f45-124">[userActivationCounts](../resources/useractivationcounts.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="82f45-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="82f45-125">ユーザーの最新の製品ライセンス認証は、すべての割り当てられている製品の種類のすべてのプラットフォーム上でカウントします。</span><span class="sxs-lookup"><span data-stu-id="82f45-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82f45-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82f45-126">JSON representation</span></span>

<span data-ttu-id="82f45-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82f45-127">The following is a JSON representation of the resource.</span></span>

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
