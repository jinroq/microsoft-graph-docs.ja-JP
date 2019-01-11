---
title: mobileAppAssignment の更新
description: mobileAppAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e46df43d27e35d4d9c88a6520761d737b8bf720c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887270"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="eca3f-103">mobileAppAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="eca3f-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="eca3f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eca3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eca3f-105">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eca3f-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eca3f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eca3f-106">Prerequisites</span></span>
<span data-ttu-id="eca3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eca3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eca3f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eca3f-109">Permission type</span></span>|<span data-ttu-id="eca3f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eca3f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eca3f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eca3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eca3f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eca3f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eca3f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eca3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eca3f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eca3f-114">Not supported.</span></span>|
|<span data-ttu-id="eca3f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eca3f-115">Application</span></span>|<span data-ttu-id="eca3f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eca3f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eca3f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eca3f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eca3f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eca3f-118">Request headers</span></span>
|<span data-ttu-id="eca3f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eca3f-119">Header</span></span>|<span data-ttu-id="eca3f-120">値</span><span class="sxs-lookup"><span data-stu-id="eca3f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eca3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eca3f-121">Authorization</span></span>|<span data-ttu-id="eca3f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="eca3f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eca3f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eca3f-123">Accept</span></span>|<span data-ttu-id="eca3f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eca3f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eca3f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eca3f-125">Request body</span></span>
<span data-ttu-id="eca3f-126">要求本文で、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eca3f-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="eca3f-127">次の表に、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eca3f-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="eca3f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eca3f-128">Property</span></span>|<span data-ttu-id="eca3f-129">種類</span><span class="sxs-lookup"><span data-stu-id="eca3f-129">Type</span></span>|<span data-ttu-id="eca3f-130">説明</span><span class="sxs-lookup"><span data-stu-id="eca3f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca3f-131">ID</span><span class="sxs-lookup"><span data-stu-id="eca3f-131">id</span></span>|<span data-ttu-id="eca3f-132">String</span><span class="sxs-lookup"><span data-stu-id="eca3f-132">String</span></span>|<span data-ttu-id="eca3f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="eca3f-133">Key of the entity.</span></span>|
|<span data-ttu-id="eca3f-134">intent</span><span class="sxs-lookup"><span data-stu-id="eca3f-134">intent</span></span>|[<span data-ttu-id="eca3f-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="eca3f-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="eca3f-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="eca3f-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="eca3f-137">target</span><span class="sxs-lookup"><span data-stu-id="eca3f-137">target</span></span>|[<span data-ttu-id="eca3f-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eca3f-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eca3f-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="eca3f-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="eca3f-140">settings</span><span class="sxs-lookup"><span data-stu-id="eca3f-140">settings</span></span>|[<span data-ttu-id="eca3f-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="eca3f-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="eca3f-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="eca3f-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="eca3f-143">応答</span><span class="sxs-lookup"><span data-stu-id="eca3f-143">Response</span></span>
<span data-ttu-id="eca3f-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eca3f-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eca3f-145">例</span><span class="sxs-lookup"><span data-stu-id="eca3f-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="eca3f-146">要求</span><span class="sxs-lookup"><span data-stu-id="eca3f-146">Request</span></span>
<span data-ttu-id="eca3f-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eca3f-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="eca3f-148">応答</span><span class="sxs-lookup"><span data-stu-id="eca3f-148">Response</span></span>
<span data-ttu-id="eca3f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eca3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



