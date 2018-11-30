---
title: Planner でオーダー ヒントを使用する
description: '`)'
ms.openlocfilehash: eaacbcad509fd778990f7f73834897ff6cf79e15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023516"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="8ee7e-103">Planner でオーダー ヒントを使用する</span><span class="sxs-lookup"><span data-stu-id="8ee7e-103">Using order hints in Planner</span></span>

<span data-ttu-id="8ee7e-p101">オーダー ヒントによって、Planner 内のオブジェクトの並べ替え順序を特定します。オーダー ヒントの値は文字列です。クライアントは項目の順序を特定するため、文字の序数値に基づいて文字列を並べ替えることができます。文字の序数値に違いが発生するまで、または文字列の終わりまで、文字列の先頭から文字を比較します。後者の場合、短い方の文字列を長い文字列より前に並べ替えます。値には、32 (スペース) から 126 (`~`) の序数のうち、どの文字でも含めることができます</span><span class="sxs-lookup"><span data-stu-id="8ee7e-p101">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="8ee7e-p102">一例として、オーダー ヒント `a` (序数値 97) を持つ項目は、オーダー ヒント `z` (序数値 122) を持つ別の項目より前に配置されます。オーダー ヒント `abc` (序数値 97、98、99) を持つ項目は、オーダー ヒント `abd` (序数値 97、98、100) を持つ別の項目より前に配置されます。オーダー ヒント `a` を持つ項目は、オーダー ヒント `ab` を持つ別の項目より前に配置されますが、これは存在するすべての文字が同じであり、`a` の方が短いためです。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-p102">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="8ee7e-p103">このサービスにより、すべてのオーダー ヒントの値を計算します。クライアントは、2 つの項目間を移動した項目のオーダー ヒントを指定することによって、項目を並べ替えることができます。オーダー ヒントを次の値に設定します。`<previous order hint> <next order hint>!`、ここでは新しく要求した場所の前に来る項目のオーダー ヒントによって `<previous order hint>` が置き換えられ、新しく要求した場所の後に来る項目のオーダー ヒントによって `<next order hint>` が置き換えられます。これらのオーダー ヒントの値の間には空白文字があり、値全体の後に `!` が付きます。いずれの項目も存在しない場合は、代わりに空の文字列を使用する必要があります。この値は以前の計算で構成することもでき、オーダー ヒントを返したサービスと全く同じように項目を並べ替えるためにクライアントで使用することもできます。更新プログラムでクライアントがこれらの値を送信したら、このサービスは要求された場所で並べ替えを行う短い値を計算します。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-p103">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

<span data-ttu-id="8ee7e-118">**注意：** 次の例では意味を明確にするために、実際のオーダー ヒントの値が一重引用符 (`'`) で囲まれていますが、これらはデータの一部ではないため、サービスに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-118">**Please note** that in the following examples the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="8ee7e-119">たとえば、以下のオーダー ヒントの並べ替えのリストについて検討します。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-119">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="8ee7e-120">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-120">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="8ee7e-121">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-121">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="8ee7e-122">項目 3 を項目 1 の前に配置し、次に項目 4 を項目 1 と項目 2 の間に配置します。次いで項目 5 を項目 2 の後に配置すれば、クライアント上で以下のオーダー ヒントが作成されます。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-122">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="8ee7e-123">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-123">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="8ee7e-124">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-124">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="8ee7e-125">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-125">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="8ee7e-126">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-126">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="8ee7e-127">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-127">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="8ee7e-128">次に、項目 1 をリストの末尾に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-128">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="8ee7e-129">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-129">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="8ee7e-130">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-130">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="8ee7e-131">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-131">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="8ee7e-132">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-132">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="8ee7e-133">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-133">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="8ee7e-134">最後に、項目 5 を項目 3 と項目 4 の間に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-134">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="8ee7e-135">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-135">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="8ee7e-136">項目 5 (オーダー ヒント: `' 5637! 5637 adhg!!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-136">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="8ee7e-137">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-137">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="8ee7e-138">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-138">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="8ee7e-139">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-139">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="8ee7e-p104">オーダー ヒントの値に対するこれらの変更がパッチ要求のサービスに送信されると、サービスはクライアントが意図した順序を保持するための適切な値を計算します。`PATCH` 要求で `return=representation` の設定が指定されている場合、クライアントは即時に値を取得できます。上記の場合の値は、次のように表示されます (実際の値は異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-p104">Once these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client. The client can obtain the values immediate if `return=representation` preference is specified in the `PATCH` requests. The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="8ee7e-143">項目 3 (オーダー ヒント: `'432b'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-143">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="8ee7e-144">項目 5 (オーダー ヒント: `'6F"#'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-144">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="8ee7e-145">項目 4 (オーダー ヒント: `'7A$6'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-145">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="8ee7e-146">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-146">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="8ee7e-147">項目 1 (オーダー ヒント: `'de5%'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-147">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="8ee7e-p105">リストの最初の項目を作成する場合、前または次の項目がいずれも存在しないため、オーダー ヒントを ` !` として指定することができます。ただし、項目の作成時にオーダー ヒントの値が指定されない場合、そうする必要はありません。これは、サービスが項目のすべてのオーダー ヒントの値を自動生成するためです。次の例は、以前に空白だったリストに項目を配置する場合、オーダー ヒントを使用する必要があることを示しています。最初の項目を追加します。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-p105">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="8ee7e-151">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-151">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="8ee7e-152">2 番目の項目を先頭に追加します。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-152">Add the second item to top:</span></span>

1. <span data-ttu-id="8ee7e-153">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-153">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="8ee7e-154">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-154">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="8ee7e-155">3 番目の項目を一番下に追加します。</span><span class="sxs-lookup"><span data-stu-id="8ee7e-155">Add the third item to bottom:</span></span>

1. <span data-ttu-id="8ee7e-156">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-156">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="8ee7e-157">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-157">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="8ee7e-158">項目 3 (オーダー ヒント: `' ! !'`)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-158">Item 3 (Order Hint: `' ! !'`)</span></span>







