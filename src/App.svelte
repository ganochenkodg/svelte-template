<script>
	import axios from 'axios';
	import {
		Button,
		Col,
		Row,
		Modal,
		ModalBody,
		ModalFooter,
		ModalHeader,
		Input,
		Label
	} from 'sveltestrap';
	import {
		onMount
	} from "svelte";
	let open = false;
	function toggle() {
		open = !open;
	};
</script>

<div>
	<Button color="success" on:click={toggle}>Demo modal</Button>
	<Modal isOpen={open} {toggle}>
		<ModalHeader {toggle}>Demo modal</ModalHeader>
		<ModalBody>
		  <Label for="newTitle">Demo:</Label>
		  <Input type="text" placeholder="demo"/>
			<p></p>
		</ModalBody>
		<ModalFooter>
			<Button color="primary" on:click={toggle}>
				OK
			</Button>
			<Button color="secondary" on:click={toggle}>
				Cancel
			</Button>
		</ModalFooter>
	</Modal>
</div>
