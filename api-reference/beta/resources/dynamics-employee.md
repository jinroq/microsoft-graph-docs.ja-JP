---
title: employees リソースの種類
description: Dynamics 365 Business Central の employee オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 96d44856ad52c983e61181fc64b93477fbe79e6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972951"
---
# <a name="employees-resource-type"></a><span data-ttu-id="e5d56-103">employees リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5d56-103">employees resource type</span></span>
<span data-ttu-id="e5d56-104">Dynamics 365 Business Central の従業員を表します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e5d56-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5d56-105">Methods</span></span>

| <span data-ttu-id="e5d56-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5d56-106">Method</span></span>                                              | <span data-ttu-id="e5d56-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5d56-107">Return Type</span></span>|<span data-ttu-id="e5d56-108">説明</span><span class="sxs-lookup"><span data-stu-id="e5d56-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="e5d56-109">従業員の取得</span><span class="sxs-lookup"><span data-stu-id="e5d56-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="e5d56-110">向け</span><span class="sxs-lookup"><span data-stu-id="e5d56-110">employees</span></span>  |<span data-ttu-id="e5d56-111">Employee オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="e5d56-112">従業員の投稿</span><span class="sxs-lookup"><span data-stu-id="e5d56-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="e5d56-113">向け</span><span class="sxs-lookup"><span data-stu-id="e5d56-113">employees</span></span>  |<span data-ttu-id="e5d56-114">Employee オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-114">Create an employee object.</span></span>|
|[<span data-ttu-id="e5d56-115">パッチの従業員</span><span class="sxs-lookup"><span data-stu-id="e5d56-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="e5d56-116">向け</span><span class="sxs-lookup"><span data-stu-id="e5d56-116">employees</span></span>  |<span data-ttu-id="e5d56-117">Employee オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-117">Update an employee object.</span></span>|
|[<span data-ttu-id="e5d56-118">従業員を削除する</span><span class="sxs-lookup"><span data-stu-id="e5d56-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="e5d56-119">none</span><span class="sxs-lookup"><span data-stu-id="e5d56-119">none</span></span>       |<span data-ttu-id="e5d56-120">Employee オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5d56-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5d56-121">Properties</span></span>
| <span data-ttu-id="e5d56-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5d56-122">Property</span></span>           | <span data-ttu-id="e5d56-123">型</span><span class="sxs-lookup"><span data-stu-id="e5d56-123">Type</span></span>   |<span data-ttu-id="e5d56-124">説明</span><span class="sxs-lookup"><span data-stu-id="e5d56-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="e5d56-125">id</span><span class="sxs-lookup"><span data-stu-id="e5d56-125">id</span></span>                  |<span data-ttu-id="e5d56-126">GUID</span><span class="sxs-lookup"><span data-stu-id="e5d56-126">GUID</span></span>    |<span data-ttu-id="e5d56-127">従業員 ID。</span><span class="sxs-lookup"><span data-stu-id="e5d56-127">The employee ID.</span></span> <span data-ttu-id="e5d56-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="e5d56-128">Non-editable.</span></span>                         |
|<span data-ttu-id="e5d56-129">番号</span><span class="sxs-lookup"><span data-stu-id="e5d56-129">number</span></span>              |<span data-ttu-id="e5d56-130">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-130">string</span></span>  |<span data-ttu-id="e5d56-131">従業員番号。</span><span class="sxs-lookup"><span data-stu-id="e5d56-131">The employee number.</span></span> <span data-ttu-id="e5d56-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5d56-132">Read-Only.</span></span>                        |
|<span data-ttu-id="e5d56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e5d56-133">displayName</span></span>         |<span data-ttu-id="e5d56-134">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-134">string</span></span>  |<span data-ttu-id="e5d56-135">従業員の givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="e5d56-135">The employee givenName + surname.</span></span> <span data-ttu-id="e5d56-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5d56-136">Read-Only.</span></span>           |
|<span data-ttu-id="e5d56-137">givenName</span><span class="sxs-lookup"><span data-stu-id="e5d56-137">givenName</span></span>           |<span data-ttu-id="e5d56-138">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-138">string</span></span>  |<span data-ttu-id="e5d56-139">従業員の指定された名前。</span><span class="sxs-lookup"><span data-stu-id="e5d56-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="e5d56-140">middleName</span><span class="sxs-lookup"><span data-stu-id="e5d56-140">middleName</span></span>          |<span data-ttu-id="e5d56-141">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-141">string</span></span>  |<span data-ttu-id="e5d56-142">従業員のミドルネーム。</span><span class="sxs-lookup"><span data-stu-id="e5d56-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="e5d56-143">surname</span><span class="sxs-lookup"><span data-stu-id="e5d56-143">surname</span></span>             |<span data-ttu-id="e5d56-144">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-144">string</span></span>  |<span data-ttu-id="e5d56-145">従業員の姓</span><span class="sxs-lookup"><span data-stu-id="e5d56-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="e5d56-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e5d56-146">jobTitle</span></span>            |<span data-ttu-id="e5d56-147">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-147">string</span></span>  |<span data-ttu-id="e5d56-148">従業員の正式な名前</span><span class="sxs-lookup"><span data-stu-id="e5d56-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="e5d56-149">address</span><span class="sxs-lookup"><span data-stu-id="e5d56-149">address</span></span>             |[<span data-ttu-id="e5d56-150">ナビゲーション."Postaladdress</span><span class="sxs-lookup"><span data-stu-id="e5d56-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="e5d56-151">従業員の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-151">Specifies the employee's address.</span></span> <span data-ttu-id="e5d56-152">このアドレスは、従業員のすべてのリソースドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e5d56-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="e5d56-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e5d56-153">phoneNumber</span></span>         |<span data-ttu-id="e5d56-154">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-154">string</span></span>  |<span data-ttu-id="e5d56-155">従業員の電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="e5d56-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e5d56-156">mobilePhone</span></span>         |<span data-ttu-id="e5d56-157">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-157">string</span></span>  |<span data-ttu-id="e5d56-158">従業員の携帯電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="e5d56-159">email</span><span class="sxs-lookup"><span data-stu-id="e5d56-159">email</span></span>               |<span data-ttu-id="e5d56-160">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-160">string</span></span>  |<span data-ttu-id="e5d56-161">従業員の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="e5d56-162">パーソナル電子メール</span><span class="sxs-lookup"><span data-stu-id="e5d56-162">personalEmail</span></span>       |<span data-ttu-id="e5d56-163">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-163">string</span></span>  |<span data-ttu-id="e5d56-164">従業員の個人の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="e5d56-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="e5d56-165">employmentDate</span></span>      |<span data-ttu-id="e5d56-166">date</span><span class="sxs-lookup"><span data-stu-id="e5d56-166">date</span></span>    |<span data-ttu-id="e5d56-167">従業員が会社の作業を開始した日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="e5d56-168">終了した日付</span><span class="sxs-lookup"><span data-stu-id="e5d56-168">terminationDate</span></span>     |<span data-ttu-id="e5d56-169">date</span><span class="sxs-lookup"><span data-stu-id="e5d56-169">date</span></span>    |<span data-ttu-id="e5d56-170">退職または棄却のために従業員が終了した日付を指定します (例:)。</span><span class="sxs-lookup"><span data-stu-id="e5d56-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="e5d56-171">status</span><span class="sxs-lookup"><span data-stu-id="e5d56-171">status</span></span>              |<span data-ttu-id="e5d56-172">string</span><span class="sxs-lookup"><span data-stu-id="e5d56-172">string</span></span>  |<span data-ttu-id="e5d56-173">従業員の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-173">Specifies the employee's status.</span></span> <span data-ttu-id="e5d56-174">有効な値、非アクティブな値、または終了した値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="e5d56-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="e5d56-175">birthDate</span></span>           |<span data-ttu-id="e5d56-176">date</span><span class="sxs-lookup"><span data-stu-id="e5d56-176">date</span></span>    |<span data-ttu-id="e5d56-177">従業員の生年月日を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5d56-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="e5d56-178">表</span><span class="sxs-lookup"><span data-stu-id="e5d56-178">picture</span></span>             |<span data-ttu-id="e5d56-179">stream</span><span class="sxs-lookup"><span data-stu-id="e5d56-179">stream</span></span>  |<span data-ttu-id="e5d56-180">従業員の画像。</span><span class="sxs-lookup"><span data-stu-id="e5d56-180">The employee picture.</span></span> <span data-ttu-id="e5d56-181">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5d56-181">Read-Only.</span></span>                       |
|<span data-ttu-id="e5d56-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d56-182">lastModifiedDateTime</span></span>|<span data-ttu-id="e5d56-183">datetime</span><span class="sxs-lookup"><span data-stu-id="e5d56-183">datetime</span></span>|<span data-ttu-id="e5d56-184">従業員が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e5d56-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="e5d56-185">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e5d56-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="e5d56-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5d56-186">Relationships</span></span>
<span data-ttu-id="e5d56-187">なし</span><span class="sxs-lookup"><span data-stu-id="e5d56-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d56-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5d56-188">JSON representation</span></span>

<span data-ttu-id="e5d56-189">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5d56-189">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

