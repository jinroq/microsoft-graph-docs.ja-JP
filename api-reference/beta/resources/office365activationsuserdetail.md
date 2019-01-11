---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: f87a5b32b08466428f0f6f0246a4b8d4c20e97be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877337"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="03618-103">office365ActivationsUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03618-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="03618-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03618-104">Properties</span></span>

| <span data-ttu-id="03618-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03618-105">Property</span></span>             | <span data-ttu-id="03618-106">種類</span><span class="sxs-lookup"><span data-stu-id="03618-106">Type</span></span>                                     | <span data-ttu-id="03618-107">説明</span><span class="sxs-lookup"><span data-stu-id="03618-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="03618-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="03618-108">reportRefreshDate</span></span>    | <span data-ttu-id="03618-109">日付</span><span class="sxs-lookup"><span data-stu-id="03618-109">Date</span></span>                                     | <span data-ttu-id="03618-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="03618-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="03618-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03618-111">userPrincipalName</span></span>    | <span data-ttu-id="03618-112">String</span><span class="sxs-lookup"><span data-stu-id="03618-112">String</span></span>                                   | <span data-ttu-id="03618-113">ユーザー プリンシパル名 (UPN) のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="03618-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="03618-114">UPN は、インターネット標準の RFC 822 に基づくユーザーに対して、インターネット スタイルのログイン名です。</span><span class="sxs-lookup"><span data-stu-id="03618-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="03618-115">規則では、これはユーザーの電子メール名にマップする必要があります。</span><span class="sxs-lookup"><span data-stu-id="03618-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="03618-116">一般的な形式は、ドメインをドメインの検証済みのテナントのコレクション内に存在する必要があります、alias@domain、です。</span><span class="sxs-lookup"><span data-stu-id="03618-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="03618-117">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="03618-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="03618-118">displayName</span><span class="sxs-lookup"><span data-stu-id="03618-118">displayName</span></span>          | <span data-ttu-id="03618-119">String</span><span class="sxs-lookup"><span data-stu-id="03618-119">String</span></span>                                   | <span data-ttu-id="03618-120">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="03618-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="03618-121">これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。</span><span class="sxs-lookup"><span data-stu-id="03618-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="03618-122">このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="03618-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="03618-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="03618-123">userActivationCounts</span></span> | <span data-ttu-id="03618-124">[userActivationCounts](../resources/useractivationcounts.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="03618-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="03618-125">ユーザーの最新の製品ライセンス認証は、すべての割り当てられている製品の種類のすべてのプラットフォーム上でカウントします。</span><span class="sxs-lookup"><span data-stu-id="03618-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03618-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03618-126">JSON representation</span></span>

<span data-ttu-id="03618-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03618-127">The following is a JSON representation of the resource.</span></span>

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
