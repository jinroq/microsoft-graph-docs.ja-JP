---
title: implicitGrantSettings リソースの種類
description: この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。 暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。 暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。
ms.openlocfilehash: 018cd422b56724811e1913ff0e94aea16d7c68f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068806"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="fb852-105">implicitGrantSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb852-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="fb852-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb852-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb852-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb852-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb852-108">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb852-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="fb852-109">暗黙の流れの一部として、ID とアクセス トークンを要求する別のプロパティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="fb852-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="fb852-110">暗黙のフローを有効にするには、次のプロパティの少なくとも 1 つ設定する必要がある true に設定します。</span><span class="sxs-lookup"><span data-stu-id="fb852-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="fb852-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb852-111">Properties</span></span>

| <span data-ttu-id="fb852-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb852-112">Property</span></span> | <span data-ttu-id="fb852-113">型</span><span class="sxs-lookup"><span data-stu-id="fb852-113">Type</span></span> | <span data-ttu-id="fb852-114">説明</span><span class="sxs-lookup"><span data-stu-id="fb852-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="fb852-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="fb852-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="fb852-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="fb852-116">Boolean</span></span> | <span data-ttu-id="fb852-117">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用して ID トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb852-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="fb852-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="fb852-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="fb852-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="fb852-119">Boolean</span></span> | <span data-ttu-id="fb852-120">この web アプリケーションで、OAuth 2.0 の暗黙的なフローを使用してアクセス トークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb852-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb852-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb852-121">JSON representation</span></span>
<span data-ttu-id="fb852-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb852-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
