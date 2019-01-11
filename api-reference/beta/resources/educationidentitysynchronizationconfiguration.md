---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c04233dd7f0383d238f0a7e7245e9451fb764be6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869063"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="8bca9-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bca9-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="8bca9-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bca9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bca9-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bca9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bca9-108">すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="8bca9-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="8bca9-109">派生クラスは、識別情報を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="8bca9-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="8bca9-110">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bca9-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8bca9-111">派生型</span><span class="sxs-lookup"><span data-stu-id="8bca9-111">Derived types</span></span>
| <span data-ttu-id="8bca9-112">Type</span><span class="sxs-lookup"><span data-stu-id="8bca9-112">Type</span></span> | <span data-ttu-id="8bca9-113">説明</span><span class="sxs-lookup"><span data-stu-id="8bca9-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="8bca9-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="8bca9-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="8bca9-115">Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="8bca9-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="8bca9-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="8bca9-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="8bca9-117">Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="8bca9-117">Use this type to create new user accounts in Azure AD.</span></span> |
