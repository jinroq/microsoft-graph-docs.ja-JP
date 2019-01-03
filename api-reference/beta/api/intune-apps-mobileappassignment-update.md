---
title: mobileAppAssignment の更新
description: mobileAppAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: ee6a6de3d20257121721ccb94f316230db8112d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361118"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="7c024-103">mobileAppAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7c024-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="7c024-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c024-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c024-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c024-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c024-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c024-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c024-107">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7c024-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c024-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c024-108">Prerequisites</span></span>
<span data-ttu-id="7c024-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c024-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c024-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c024-111">Permission type</span></span>|<span data-ttu-id="7c024-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c024-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c024-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c024-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c024-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c024-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c024-116">Not supported.</span></span>|
|<span data-ttu-id="7c024-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c024-117">Application</span></span>|<span data-ttu-id="7c024-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c024-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c024-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7c024-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c024-120">Request headers</span></span>
|<span data-ttu-id="7c024-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c024-121">Header</span></span>|<span data-ttu-id="7c024-122">値</span><span class="sxs-lookup"><span data-stu-id="7c024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c024-123">Authorization</span></span>|<span data-ttu-id="7c024-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c024-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c024-125">Accept</span></span>|<span data-ttu-id="7c024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c024-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c024-127">Request body</span></span>
<span data-ttu-id="7c024-128">要求本文で、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c024-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="7c024-129">次の表に、[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c024-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="7c024-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c024-130">Property</span></span>|<span data-ttu-id="7c024-131">種類</span><span class="sxs-lookup"><span data-stu-id="7c024-131">Type</span></span>|<span data-ttu-id="7c024-132">説明</span><span class="sxs-lookup"><span data-stu-id="7c024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c024-133">ID</span><span class="sxs-lookup"><span data-stu-id="7c024-133">id</span></span>|<span data-ttu-id="7c024-134">String</span><span class="sxs-lookup"><span data-stu-id="7c024-134">String</span></span>|<span data-ttu-id="7c024-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7c024-135">Key of the entity.</span></span>|
|<span data-ttu-id="7c024-136">intent</span><span class="sxs-lookup"><span data-stu-id="7c024-136">intent</span></span>|[<span data-ttu-id="7c024-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="7c024-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7c024-138">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="7c024-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="7c024-139">target</span><span class="sxs-lookup"><span data-stu-id="7c024-139">target</span></span>|[<span data-ttu-id="7c024-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c024-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7c024-141">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="7c024-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="7c024-142">settings</span><span class="sxs-lookup"><span data-stu-id="7c024-142">settings</span></span>|[<span data-ttu-id="7c024-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7c024-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="7c024-144">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="7c024-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="7c024-145">応答</span><span class="sxs-lookup"><span data-stu-id="7c024-145">Response</span></span>
<span data-ttu-id="7c024-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c024-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c024-147">例</span><span class="sxs-lookup"><span data-stu-id="7c024-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c024-148">要求</span><span class="sxs-lookup"><span data-stu-id="7c024-148">Request</span></span>
<span data-ttu-id="7c024-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c024-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 215

{
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="7c024-150">応答</span><span class="sxs-lookup"><span data-stu-id="7c024-150">Response</span></span>
<span data-ttu-id="7c024-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c024-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




