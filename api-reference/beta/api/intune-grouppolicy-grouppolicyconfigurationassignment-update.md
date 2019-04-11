---
title: grouppolicyconfigurationassignment の更新
description: grouppolicyconfigurationassignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1306abca31be57b71b883b7fdaa5d2e8ab47fec4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780540"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="c4e16-103">grouppolicyconfigurationassignment の更新</span><span class="sxs-lookup"><span data-stu-id="c4e16-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="c4e16-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4e16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4e16-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4e16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4e16-106">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4e16-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4e16-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4e16-107">Prerequisites</span></span>
<span data-ttu-id="c4e16-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4e16-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4e16-110">Permission type</span></span>|<span data-ttu-id="c4e16-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4e16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4e16-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4e16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4e16-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4e16-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4e16-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4e16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4e16-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4e16-115">Not supported.</span></span>|
|<span data-ttu-id="c4e16-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4e16-116">Application</span></span>|<span data-ttu-id="c4e16-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4e16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4e16-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4e16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c4e16-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4e16-119">Request headers</span></span>
|<span data-ttu-id="c4e16-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4e16-120">Header</span></span>|<span data-ttu-id="c4e16-121">値</span><span class="sxs-lookup"><span data-stu-id="c4e16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4e16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4e16-122">Authorization</span></span>|<span data-ttu-id="c4e16-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4e16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4e16-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c4e16-124">Accept</span></span>|<span data-ttu-id="c4e16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4e16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4e16-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4e16-126">Request body</span></span>
<span data-ttu-id="c4e16-127">要求本文で、 [grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4e16-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c4e16-128">次の表に、 [grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c4e16-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="c4e16-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4e16-129">Property</span></span>|<span data-ttu-id="c4e16-130">型</span><span class="sxs-lookup"><span data-stu-id="c4e16-130">Type</span></span>|<span data-ttu-id="c4e16-131">説明</span><span class="sxs-lookup"><span data-stu-id="c4e16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4e16-132">id</span><span class="sxs-lookup"><span data-stu-id="c4e16-132">id</span></span>|<span data-ttu-id="c4e16-133">String</span><span class="sxs-lookup"><span data-stu-id="c4e16-133">String</span></span>|<span data-ttu-id="c4e16-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c4e16-134">Key of the entity.</span></span>|
|<span data-ttu-id="c4e16-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4e16-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c4e16-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4e16-136">DateTimeOffset</span></span>|<span data-ttu-id="c4e16-137">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c4e16-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c4e16-138">target</span><span class="sxs-lookup"><span data-stu-id="c4e16-138">target</span></span>|[<span data-ttu-id="c4e16-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c4e16-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c4e16-140">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="c4e16-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c4e16-141">応答</span><span class="sxs-lookup"><span data-stu-id="c4e16-141">Response</span></span>
<span data-ttu-id="c4e16-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4e16-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4e16-143">例</span><span class="sxs-lookup"><span data-stu-id="c4e16-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4e16-144">要求</span><span class="sxs-lookup"><span data-stu-id="c4e16-144">Request</span></span>
<span data-ttu-id="c4e16-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4e16-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c4e16-146">応答</span><span class="sxs-lookup"><span data-stu-id="c4e16-146">Response</span></span>
<span data-ttu-id="c4e16-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4e16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





