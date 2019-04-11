---
title: grouppolicyconfigurationassignment の作成
description: 新しい grouppolicyconfigurationassignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b0deda8c76a52705a60787766711b18b4b6ff50
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780610"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="69cb5-103">grouppolicyconfigurationassignment の作成</span><span class="sxs-lookup"><span data-stu-id="69cb5-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="69cb5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69cb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69cb5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69cb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69cb5-106">新しい[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="69cb5-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69cb5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="69cb5-107">Prerequisites</span></span>
<span data-ttu-id="69cb5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69cb5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69cb5-110">Permission type</span></span>|<span data-ttu-id="69cb5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69cb5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69cb5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69cb5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69cb5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69cb5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="69cb5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69cb5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69cb5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69cb5-115">Not supported.</span></span>|
|<span data-ttu-id="69cb5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69cb5-116">Application</span></span>|<span data-ttu-id="69cb5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69cb5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69cb5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69cb5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="69cb5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69cb5-119">Request headers</span></span>
|<span data-ttu-id="69cb5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69cb5-120">Header</span></span>|<span data-ttu-id="69cb5-121">値</span><span class="sxs-lookup"><span data-stu-id="69cb5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69cb5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69cb5-122">Authorization</span></span>|<span data-ttu-id="69cb5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="69cb5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69cb5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="69cb5-124">Accept</span></span>|<span data-ttu-id="69cb5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69cb5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69cb5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="69cb5-126">Request body</span></span>
<span data-ttu-id="69cb5-127">要求本文で、grouppolicyconfigurationassignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69cb5-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="69cb5-128">次の表に、grouppolicyconfigurationassignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69cb5-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="69cb5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69cb5-129">Property</span></span>|<span data-ttu-id="69cb5-130">型</span><span class="sxs-lookup"><span data-stu-id="69cb5-130">Type</span></span>|<span data-ttu-id="69cb5-131">説明</span><span class="sxs-lookup"><span data-stu-id="69cb5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cb5-132">id</span><span class="sxs-lookup"><span data-stu-id="69cb5-132">id</span></span>|<span data-ttu-id="69cb5-133">String</span><span class="sxs-lookup"><span data-stu-id="69cb5-133">String</span></span>|<span data-ttu-id="69cb5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="69cb5-134">Key of the entity.</span></span>|
|<span data-ttu-id="69cb5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69cb5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="69cb5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69cb5-136">DateTimeOffset</span></span>|<span data-ttu-id="69cb5-137">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="69cb5-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="69cb5-138">target</span><span class="sxs-lookup"><span data-stu-id="69cb5-138">target</span></span>|[<span data-ttu-id="69cb5-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="69cb5-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="69cb5-140">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="69cb5-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="69cb5-141">応答</span><span class="sxs-lookup"><span data-stu-id="69cb5-141">Response</span></span>
<span data-ttu-id="69cb5-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69cb5-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69cb5-143">例</span><span class="sxs-lookup"><span data-stu-id="69cb5-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="69cb5-144">要求</span><span class="sxs-lookup"><span data-stu-id="69cb5-144">Request</span></span>
<span data-ttu-id="69cb5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69cb5-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="69cb5-146">応答</span><span class="sxs-lookup"><span data-stu-id="69cb5-146">Response</span></span>
<span data-ttu-id="69cb5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69cb5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





