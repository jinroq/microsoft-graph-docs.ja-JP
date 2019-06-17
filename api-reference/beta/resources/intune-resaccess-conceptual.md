---
title: Intune でリソースアクセス証明書を管理する-Microsoft Graph API
description: テナント組織のリソースアクセス証明書を管理する Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed680af82eb041e93cf73cb6ed3c390b989d8bc3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996261"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="fd61a-103">Intune でリソースアクセス証明書を管理する</span><span class="sxs-lookup"><span data-stu-id="fd61a-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="fd61a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd61a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd61a-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd61a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd61a-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd61a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd61a-107">Microsoft Graph API for Intune を使用して、PFX 証明書をインポートできます。</span><span class="sxs-lookup"><span data-stu-id="fd61a-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="fd61a-108">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="fd61a-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="fd61a-109">ユーザーの PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="fd61a-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="fd61a-110">ユーザー PFX の目的</span><span class="sxs-lookup"><span data-stu-id="fd61a-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="fd61a-111">ユーザーの PFX 埋め込みスキーム</span><span class="sxs-lookup"><span data-stu-id="fd61a-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
