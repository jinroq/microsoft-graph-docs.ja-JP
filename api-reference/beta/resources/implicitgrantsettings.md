---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。
localization_priority: Normal
ms.openlocfilehash: 93a54ac0c0e4c6c32ebb99c9747d44d75f98af07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834266"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="55c5c-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55c5c-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="55c5c-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55c5c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55c5c-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55c5c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55c5c-108">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="55c5c-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="55c5c-109">暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="55c5c-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="55c5c-110">暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。</span><span class="sxs-lookup"><span data-stu-id="55c5c-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="55c5c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55c5c-111">Properties</span></span>

| <span data-ttu-id="55c5c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55c5c-112">Property</span></span> | <span data-ttu-id="55c5c-113">種類</span><span class="sxs-lookup"><span data-stu-id="55c5c-113">Type</span></span> | <span data-ttu-id="55c5c-114">説明</span><span class="sxs-lookup"><span data-stu-id="55c5c-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="55c5c-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="55c5c-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="55c5c-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="55c5c-116">Boolean</span></span> | <span data-ttu-id="55c5c-117">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="55c5c-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="55c5c-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="55c5c-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="55c5c-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="55c5c-119">Boolean</span></span> | <span data-ttu-id="55c5c-120">この web アプリケーションで、OAuth 2.0 の暗黙的なフローを使用してアクセス トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="55c5c-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55c5c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55c5c-121">JSON representation</span></span>
<span data-ttu-id="55c5c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55c5c-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
