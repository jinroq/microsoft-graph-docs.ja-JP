---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、システムはプロバイダ api への接続方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334115"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="fc5cc-104">educationSynchronizationConnectionSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc5cc-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc5cc-105">プロバイダー接続の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-105">Represents the provider connection settings.</span></span> <span data-ttu-id="fc5cc-106">これにより、システムはプロバイダ api への接続方法を知ることができます。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="fc5cc-107">**注:** この複合型は抽象型です。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="fc5cc-108">一覧にある特定の種類の接続設定を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="fc5cc-109">派生型</span><span class="sxs-lookup"><span data-stu-id="fc5cc-109">Derived types</span></span>
| <span data-ttu-id="fc5cc-110">型</span><span class="sxs-lookup"><span data-stu-id="fc5cc-110">Type</span></span> | <span data-ttu-id="fc5cc-111">説明</span><span class="sxs-lookup"><span data-stu-id="fc5cc-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="fc5cc-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="fc5cc-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="fc5cc-113">この型を使用して、OAuth1 の接続設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="fc5cc-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="fc5cc-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="fc5cc-115">この種類を使用して、OAuth2 クライアント資格情報の付与に接続設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc5cc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc5cc-116">Properties</span></span>

| <span data-ttu-id="fc5cc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc5cc-117">Property</span></span> | <span data-ttu-id="fc5cc-118">型</span><span class="sxs-lookup"><span data-stu-id="fc5cc-118">Type</span></span> | <span data-ttu-id="fc5cc-119">説明</span><span class="sxs-lookup"><span data-stu-id="fc5cc-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fc5cc-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="fc5cc-120">**clientId**</span></span> | <span data-ttu-id="fc5cc-121">String</span><span class="sxs-lookup"><span data-stu-id="fc5cc-121">String</span></span> |  <span data-ttu-id="fc5cc-122">プロバイダーへの接続に使用されるクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="fc5cc-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="fc5cc-123">**clientSecret**</span></span> | <span data-ttu-id="fc5cc-124">String</span><span class="sxs-lookup"><span data-stu-id="fc5cc-124">String</span></span> |  <span data-ttu-id="fc5cc-125">プロバイダーへの接続を認証するクライアントシークレット。</span><span class="sxs-lookup"><span data-stu-id="fc5cc-125">Client secret to authenticate the connection to the provider.</span></span> |
