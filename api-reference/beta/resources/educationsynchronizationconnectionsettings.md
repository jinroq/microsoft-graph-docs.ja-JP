---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、システムはプロバイダ Api への接続方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c82d912b13ca68dcdccd5ace0232ed65f92cd879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972490"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="54458-104">educationSynchronizationConnectionSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54458-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54458-105">プロバイダー接続の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="54458-105">Represents the provider connection settings.</span></span> <span data-ttu-id="54458-106">これにより、システムはプロバイダ Api への接続方法を知ることができます。</span><span class="sxs-lookup"><span data-stu-id="54458-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="54458-107">**注:** この複合型は抽象型です。</span><span class="sxs-lookup"><span data-stu-id="54458-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="54458-108">一覧にある特定の種類の接続設定を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54458-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="54458-109">派生型</span><span class="sxs-lookup"><span data-stu-id="54458-109">Derived types</span></span>
| <span data-ttu-id="54458-110">型</span><span class="sxs-lookup"><span data-stu-id="54458-110">Type</span></span> | <span data-ttu-id="54458-111">説明</span><span class="sxs-lookup"><span data-stu-id="54458-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="54458-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="54458-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="54458-113">この型を使用して、OAuth1 の接続設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="54458-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="54458-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="54458-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="54458-115">この種類を使用して、OAuth2 クライアント資格情報の付与に接続設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="54458-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="54458-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54458-116">Properties</span></span>

| <span data-ttu-id="54458-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54458-117">Property</span></span> | <span data-ttu-id="54458-118">型</span><span class="sxs-lookup"><span data-stu-id="54458-118">Type</span></span> | <span data-ttu-id="54458-119">説明</span><span class="sxs-lookup"><span data-stu-id="54458-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="54458-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="54458-120">**clientId**</span></span> | <span data-ttu-id="54458-121">String</span><span class="sxs-lookup"><span data-stu-id="54458-121">String</span></span> |  <span data-ttu-id="54458-122">プロバイダーへの接続に使用されるクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="54458-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="54458-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="54458-123">**clientSecret**</span></span> | <span data-ttu-id="54458-124">String</span><span class="sxs-lookup"><span data-stu-id="54458-124">String</span></span> |  <span data-ttu-id="54458-125">プロバイダーへの接続を認証するクライアントシークレット。</span><span class="sxs-lookup"><span data-stu-id="54458-125">Client secret to authenticate the connection to the provider.</span></span> |
