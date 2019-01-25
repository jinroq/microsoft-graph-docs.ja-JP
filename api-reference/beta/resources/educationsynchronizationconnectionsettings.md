---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526866"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="1bdf5-104">educationSynchronizationConnectionSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bdf5-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bdf5-105">プロバイダー接続の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-105">Represents the provider connection settings.</span></span> <span data-ttu-id="1bdf5-106">これにより、Api のプロバイダーに接続する方法を把握するシステムです。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="1bdf5-107">**注:** この複合型は抽象です。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="1bdf5-108">特定の種類の接続設定のリストを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="1bdf5-109">派生型</span><span class="sxs-lookup"><span data-stu-id="1bdf5-109">Derived types</span></span>
| <span data-ttu-id="1bdf5-110">型</span><span class="sxs-lookup"><span data-stu-id="1bdf5-110">Type</span></span> | <span data-ttu-id="1bdf5-111">説明</span><span class="sxs-lookup"><span data-stu-id="1bdf5-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="1bdf5-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="1bdf5-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="1bdf5-113">OAuth1 接続の設定を提供するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="1bdf5-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="1bdf5-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="1bdf5-115">OAuth2 クライアントの資格情報の付与の接続の設定を提供するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="1bdf5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bdf5-116">Properties</span></span>

| <span data-ttu-id="1bdf5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bdf5-117">Property</span></span> | <span data-ttu-id="1bdf5-118">型</span><span class="sxs-lookup"><span data-stu-id="1bdf5-118">Type</span></span> | <span data-ttu-id="1bdf5-119">説明</span><span class="sxs-lookup"><span data-stu-id="1bdf5-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1bdf5-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="1bdf5-120">**clientId**</span></span> | <span data-ttu-id="1bdf5-121">String</span><span class="sxs-lookup"><span data-stu-id="1bdf5-121">String</span></span> |  <span data-ttu-id="1bdf5-122">クライアント ID をプロバイダーに接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="1bdf5-123">client_secret</span><span class="sxs-lookup"><span data-stu-id="1bdf5-123">**clientSecret**</span></span> | <span data-ttu-id="1bdf5-124">String</span><span class="sxs-lookup"><span data-stu-id="1bdf5-124">String</span></span> |  <span data-ttu-id="1bdf5-125">プロバイダーへの接続を認証するためにクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="1bdf5-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
