---
title: Intune でリソースアクセス証明書を管理する-Microsoft Graph API
description: テナント組織のリソースアクセス証明書を管理する Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 943597fc6d1b133ec29e87d544c016f6c2ab703f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168139"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="19924-103">Intune でリソースアクセス証明書を管理する</span><span class="sxs-lookup"><span data-stu-id="19924-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="19924-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19924-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19924-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19924-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19924-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="19924-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="19924-107">Microsoft Graph API for Intune を使用して、PFX 証明書をインポートできます。</span><span class="sxs-lookup"><span data-stu-id="19924-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="19924-108">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="19924-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="19924-109">ユーザーの PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="19924-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="19924-110">ユーザー PFX の目的</span><span class="sxs-lookup"><span data-stu-id="19924-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="19924-111">ユーザーの PFX 埋め込みスキーム</span><span class="sxs-lookup"><span data-stu-id="19924-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
