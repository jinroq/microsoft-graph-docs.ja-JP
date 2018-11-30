---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070738"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="e58e7-104">educationSynchronizationConnectionSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e58e7-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="e58e7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e58e7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e58e7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e58e7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e58e7-107">プロバイダー接続の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="e58e7-107">Represents the provider connection settings.</span></span> <span data-ttu-id="e58e7-108">これにより、Api のプロバイダーに接続する方法を把握するシステムです。</span><span class="sxs-lookup"><span data-stu-id="e58e7-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="e58e7-109">**注:** この複合型は抽象です。</span><span class="sxs-lookup"><span data-stu-id="e58e7-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="e58e7-110">特定の種類の接続設定のリストを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e58e7-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="e58e7-111">派生型</span><span class="sxs-lookup"><span data-stu-id="e58e7-111">Derived types</span></span>
| <span data-ttu-id="e58e7-112">型</span><span class="sxs-lookup"><span data-stu-id="e58e7-112">Type</span></span> | <span data-ttu-id="e58e7-113">説明</span><span class="sxs-lookup"><span data-stu-id="e58e7-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="e58e7-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="e58e7-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="e58e7-115">OAuth1 接続の設定を提供するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="e58e7-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="e58e7-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="e58e7-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="e58e7-117">OAuth2 クライアントの資格情報の付与の接続の設定を提供するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="e58e7-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="e58e7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e58e7-118">Properties</span></span>

| <span data-ttu-id="e58e7-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e58e7-119">Property</span></span> | <span data-ttu-id="e58e7-120">型</span><span class="sxs-lookup"><span data-stu-id="e58e7-120">Type</span></span> | <span data-ttu-id="e58e7-121">説明</span><span class="sxs-lookup"><span data-stu-id="e58e7-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e58e7-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="e58e7-122">**clientId**</span></span> | <span data-ttu-id="e58e7-123">String</span><span class="sxs-lookup"><span data-stu-id="e58e7-123">String</span></span> |  <span data-ttu-id="e58e7-124">クライアント ID をプロバイダーに接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="e58e7-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="e58e7-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="e58e7-125">**clientSecret**</span></span> | <span data-ttu-id="e58e7-126">String</span><span class="sxs-lookup"><span data-stu-id="e58e7-126">String</span></span> |  <span data-ttu-id="e58e7-127">プロバイダーへの接続を認証するためにクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="e58e7-127">Client secret to authenticate the connection to the provider.</span></span> |