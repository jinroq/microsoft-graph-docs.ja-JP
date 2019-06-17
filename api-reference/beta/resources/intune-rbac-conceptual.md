---
title: Microsoft Intune での役割ベースのアクセス制御
description: テナント組織の役割ベースのアクセス制御 (RBAC) を定義して管理する Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: fe09f89a10524dc255d7e0e647ba793aec2529ab
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993661"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="b2ae4-103">Microsoft Intune での役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="b2ae4-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="b2ae4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2ae4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2ae4-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2ae4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2ae4-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2ae4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2ae4-107">Intune の役割ベースのアクセス制御により、だれが Intune オブジェクトに対してアクションを実行し、管理対象アプリケーション、ユーザー、デバイスを変更できるかが決まります。</span><span class="sxs-lookup"><span data-stu-id="b2ae4-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="b2ae4-108">次の Graph リソースを使用して、Intune での役割ベースのアクセス制御を管理できます。</span><span class="sxs-lookup"><span data-stu-id="b2ae4-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="b2ae4-109">デバイスおよびアプリ管理の割り当てられた役割の詳細</span><span class="sxs-lookup"><span data-stu-id="b2ae4-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="b2ae4-110">デバイスおよびアプリ管理役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="b2ae4-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="b2ae4-111">デバイスおよびアプリ管理役割の定義</span><span class="sxs-lookup"><span data-stu-id="b2ae4-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="b2ae4-112">リソース アクション</span><span class="sxs-lookup"><span data-stu-id="b2ae4-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="b2ae4-113">リソース操作</span><span class="sxs-lookup"><span data-stu-id="b2ae4-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="b2ae4-114">役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="b2ae4-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="b2ae4-115">ロールの割り当ての範囲のタイプ</span><span class="sxs-lookup"><span data-stu-id="b2ae4-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="b2ae4-116">役割の定義</span><span class="sxs-lookup"><span data-stu-id="b2ae4-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="b2ae4-117">役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2ae4-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="b2ae4-118">ロールの範囲のタグ</span><span class="sxs-lookup"><span data-stu-id="b2ae4-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="b2ae4-119">役割の範囲タグの自動割り当て</span><span class="sxs-lookup"><span data-stu-id="b2ae4-119">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
