---
title: extendFeatureUpdatesPause アクション
description: ビジネス リング用の Windows Update の更新一時停止の機能を拡張します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1f914eb3cd0e4cc3c3f466de2869bb61db7bc28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392494"
---
# <a name="extendfeatureupdatespause-action"></a><span data-ttu-id="5d8b6-103">extendFeatureUpdatesPause アクション</span><span class="sxs-lookup"><span data-stu-id="5d8b6-103">extendFeatureUpdatesPause action</span></span>

> <span data-ttu-id="5d8b6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d8b6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d8b6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d8b6-107">ビジネス リング用の Windows Update の更新一時停止の機能を拡張します。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-107">Extend Feature Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d8b6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5d8b6-108">Prerequisites</span></span>
<span data-ttu-id="5d8b6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d8b6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d8b6-111">Permission type</span></span>|<span data-ttu-id="5d8b6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d8b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d8b6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d8b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d8b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d8b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d8b6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d8b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d8b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-116">Not supported.</span></span>|
|<span data-ttu-id="5d8b6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d8b6-117">Application</span></span>|<span data-ttu-id="5d8b6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d8b6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d8b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="5d8b6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d8b6-120">Request headers</span></span>
|<span data-ttu-id="5d8b6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d8b6-121">Header</span></span>|<span data-ttu-id="5d8b6-122">値</span><span class="sxs-lookup"><span data-stu-id="5d8b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d8b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d8b6-123">Authorization</span></span>|<span data-ttu-id="5d8b6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d8b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d8b6-125">Accept</span></span>|<span data-ttu-id="5d8b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d8b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d8b6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d8b6-127">Request body</span></span>
<span data-ttu-id="5d8b6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d8b6-129">応答</span><span class="sxs-lookup"><span data-stu-id="5d8b6-129">Response</span></span>
<span data-ttu-id="5d8b6-130">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5d8b6-131">例</span><span class="sxs-lookup"><span data-stu-id="5d8b6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d8b6-132">要求</span><span class="sxs-lookup"><span data-stu-id="5d8b6-132">Request</span></span>
<span data-ttu-id="5d8b6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

### <a name="response"></a><span data-ttu-id="5d8b6-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d8b6-134">Response</span></span>
<span data-ttu-id="5d8b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5d8b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




