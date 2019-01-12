---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6d9841d4957d5330fc966f60a24582e101831b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969031"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="df896-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df896-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="df896-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df896-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df896-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df896-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df896-108">すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="df896-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="df896-109">派生クラスは、識別情報を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="df896-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="df896-110">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df896-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="df896-111">派生型</span><span class="sxs-lookup"><span data-stu-id="df896-111">Derived types</span></span>
| <span data-ttu-id="df896-112">Type</span><span class="sxs-lookup"><span data-stu-id="df896-112">Type</span></span> | <span data-ttu-id="df896-113">説明</span><span class="sxs-lookup"><span data-stu-id="df896-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="df896-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="df896-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="df896-115">Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="df896-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="df896-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="df896-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="df896-117">Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。</span><span class="sxs-lookup"><span data-stu-id="df896-117">Use this type to create new user accounts in Azure AD.</span></span> |
